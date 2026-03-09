---
layout: page
title: "05_House_Hunting - Discussion Summary"
permalink: /notes/05_house_hunting/discussion_summary/
---

# Discussion Summaries : House Hunting / Job Hunting / Partner Hunting

## Summary - 1:

### There was an extensive statistics and probability discussion session focused on understanding fundamental concepts through intuitive reasoning rather than complex mathematics.

### Key Topics Covered:
1. Uniform Distribution & Random Number Problems:
    - Discussed why the average of random numbers between 0 and 1 tends to be 0.5.
    - Explored the concept of placing "Diyas" (lamps) on a number line and how they naturally distribute evenly.
    - Connected this to real-world examples like birds sitting on power lines with equal spacing.

2. The German Tank Problem:
    - Estimated total population size based on observed maximum values from random samples.
    - Formula discussed: If you capture N items randomly, the expected range is N/(N+1).
    - Applied this to estimate total number of soldiers from captured uniform numbers (approximately 18,945)

3. The Secretary / Marriage Problem:
    - Discussed optimal stopping theory: when to stop searching for the best option (house, job, partner).
    - Explored the balance between gathering information and making decisions.
    - Connected to student's salary package example with 10 job offers.

4. The Biased Teacher Problem:
    - Analyzed whether a teacher selecting female CRs for 10 consecutive years was biased.
    - In a class with 90% boys and 10% girls, the probability of selecting 10 girls in a row using random selection is 1 in 10 billion.
    - Concluded that this is a strong evidence of bias.

5. Key Insights:
    - All problems relate to the same core concept: random sampling and fair distribution.
    - When dividing into K groups randomly, expect to find one from the top percentile items by checking K items of the population as it gives us a fair chance of seeing an item from the top percentile group.
    - Law of diminishing returns: doubling effort doesn't double accuracy improvement.

The discussion emphasized building intuition through real-world examples rather than jumping to formulas.

---

## Summary - 2:

### The meeting focused on developing intuitive understanding of statistical estimation through various real-world problems including house selection, job offers, and military scenarios, with participants working through concepts of percentiles, random sampling, and fairness in distribution without relying heavily on formal probability terminology.

### The group explored how the number of random observations creates bins that help estimate unknown totals, discovering that observing K data points creates K + 1 intervals with predictable minimum and maximum values, and that increasing experimental repetitions improves estimate reliability while reducing variance.

### Participants connected multiple problems including the German tank problem, teacher selection bias, and the Diya placement exercise recognizing they all share the same underlying principle of fair distribution, and began understanding how the number of trials affects estimation accuracy while the number of experiments controls confidence intervals around those estimates.

### Next Steps:
- PK: Share discussion questions 5 and 6 in the chat for participants to access and work on it.
- ACP: Lead discussion on the teacher partiality problem to help participants understand the quantification of truthfulness using probability concepts.
- KG: Present and explain the Python code demonstrating the relationship between number of trials, bin sizes, and estimation accuracy to the group in the next session.
- All participants: Work on Discussion 6 problem and understand the intuition behind the estimation formula.
- Manimator: Prepare explanation of the multiplication rule in probability using a example with two alphabets for participants who need clarification.

---

## Summary - 3:

### Detailed Meeting Summary:
### This was an extended New Year's Day 2026 coding session focused on solving a placement / package selection probability problem. The meeting had 41 speakers with primary contributors including Gurudev, JK, KG, JG, NR, DC, and others.

### Main Problem Discussion
- Core Problem Statement: The group discussed a placement scenario where:
    - A student faces 100 job offers presented sequentially in random order.
    - The student sees each salary offer one at a time.
    - They must immediately accept or reject each offer.
    - Once rejected, they cannot return to that offer.
    - Goal: Determine the optimal strategy to maximize chances of getting the best (or near-best) package.

### Key Findings and Observations
### The 37% Rule (1/e):
- Through Monte Carlo simulations with 50,000 trials, the group discovered that the optimal strategy involves observing approximately 37% of offers before making selections.
- This corresponds to the mathematical constant 1/e (approximately 0.368 or 36.8%).
- After observing this portion, one should select the next offer that exceeds all previously seen offers (or in some 5-10% range of the previously seen maximum).

### Simulation Approach:
- Participants ran experiments with varying parameters (100 offers, 1000 trials, etc.).
- The probability of success peaked around K = 37-38 (where K represents the number of offers to skip).
- Maximum success probability achieved was approximately 0.35-0.39 (35-39%).

### Technical Discussions:
### Monte Carlo Method:
Gurudev demonstrated why repeated experiments are necessary using a coin toss example, showing how probability converges to the expected value (0.3 in the example) over many iterations. This illustrated the importance of running multiple trials to achieve accuracy.

### Code Implementation Issues:
- Initial code used salaries ranging from 1 to 100.
- Later refined to use random salary generation to better represent real-world scenarios.
- Discussion about proper shuffling and random number generation.
- Debate about whether to use uniform distribution or other approaches.

---

## Summary - 4:

### Detailed Meeting Summary:
### This was an extended technical discussion session involving 15 participants from the Coder's High Club, focused on solving probability and optimization problems related to job offer selection. The meeting lasted several hours, with core discussions happening between approximately 1-2 AM.

### Main Problem Being Addressed: The team worked on the "Secretary Problem" (also called the Marriage Problem or Optimal Stopping Problem):
- A student receives N job offers (typically 10) with random salary packages.
- Offers must be accepted or rejected immediately upon receiving them.
- Once rejected, an offer cannot be revisited.
- Goal: Maximize the probability of selecting the best offer.

### Key Technical Discussions:
1. Probability Analysis (Package Threshold Problem):
- Analyzed the probability that minimum salary among 10 offers exceeds 40 lakhs.
- Package range: 1 lakh to 1 crore.
- Participants ran Monte Carlo simulations with 100,000 iterations.
- Result: Very low probability (approximately 0.73%), indicating 40 lakh is a strong offer.
- The team discussed how 10 offers divide the range into 11 equal bins on average.

2. Bin Width Estimation Strategy:
- KG proposed an innovative approach:
    - Observe consecutive offers to estimate the "bin width" (gap between offers).
    - Use minimum interval between any two observed offers to estimate theoretical maximum.
    - Formula: If K offers are seen with minimum gap G, theoretical max ≈ (K × G) / (K + 1).
    - This allows updating beliefs about the salary distribution as more offers are seen.

3. Optimal Rejection Strategy:
- The team explored the 1/e rule (approximately 37%):
    - Reject the first 37% of offers to gather information about the distribution.
    - After this exploration phase, accept the first offer that exceeds the maximum seen during exploration.
    - This balances two objectives: minimizing risk of missing the best offer vs. maximizing information gathering.

4. Risk-Reward Framework:
- Debasmit introduced a three-zone framework:
    - Rejection Zone: First K offers (exploration phase).
    - Decision Zone: Middle offers where decisions are made based on observed data.
    - Right Tail Zone: The remaining offeres which will not be seen after accepting an offer.

5. Technical Concepts Covered:
- Monte-Carlo simulations.
- Distribution analysis (minimum, maximum, bin widths).
- Risk-reward tradeoffs.
- Bayesian updating as new offers arrive.

### The meeting involved extensive coding demonstrations, probability calculations, and philosophical discussions connecting the problem to concepts from the Bhagawad Gita about doing one's duty without attachment to results.
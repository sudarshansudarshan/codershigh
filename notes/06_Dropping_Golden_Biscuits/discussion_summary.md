---
layout: page
title: "06_Dropping_Golden_Biscuits - Discussion Summary"
permalink: /notes/06_dropping_golden_biscuits/discussion_summary/
---

# Discussion Summaries : Dropping Golden Biscuits / House Bombing

## Summary - 1:

### The session focused on a probability problem involving bombs falling randomly on houses. The main discussion points were:

### Core Problem:
- If you have N houses and drop N bombs randomly, how many houses survive?
- The answer converges to N/e (approximately 36.8% of houses survive).
- Participants coded simulations to verify this result.

### Key Discoveries:
1. The number of empty (unbombed) houses follows the formula involving e (Euler's number).
2. When dropping bombs equal to the number of houses, survival probability is 1/e.
3. The maximum number of bombs a single house receives follows a pattern related to factorials.
4. The distribution of bombs per house follows a Poisson-like distribution.

### Mathematical Connections:
- The group derived that (1 - 1/N)<sup>N</sup> converges to 1/e as N increases.
- They connected this to the Taylor series expansion of e<sup>x</sup>.
- Factorial functions emerged naturally in the probability calculations.
- The limit (1 + 1/N)<sup>N</sup> = e was explored.

### Secondary Problem Discussed:
- If you drop 1ON bombs on N houses, the survival rate becomes 1/e<sup>10</sup>.
- The maximum number of bombs hitting single house is related to the factorial function threshold.

### Practical Insights:
- Participants wrote Python code to simulate and verify the theoretical results.
- They explored how the problem relates to balls-and-bins scenarios.
- Discussion touched on compound interest formulas and their connection to e.

---

## Summary - 2:

### The meeting was a collaborative discussion session focused on probability, statistics, and mathematical problem-solving. Here's a detailed summary:

### Main Topics Discussed:
1. Interactive Learning Philosophy: The session emphasized developing thinking ability over memorizing solutions. Participants were encouraged to engage actively, share ideas, and learn from each other's approaches, even if answers were wrong. The goal was to build intuition for solving novel problems.

2. Random Distribution and Fairness: The group discussed how repeated random distributions tend toward uniform distribution, demonstrating a "sense of fairness" where no particular outcome is favored.

3. The Secretary/Package Selection Problem: A major focus was on a problem about choosing the best offer from a sequence. PK shared his strategy of observing the first 10 offers to find the maximum, then selecting from remaining offers based on that benchmark. The key question became: what percentage of offers should one observe before making a decision? The discussion explored the trade-off between gaining knowledge (by observing more) and the risk of missing the best option.

4. The Bombing Problem: The group analyzed a scenario where  bombs randomly fall on houses. Key findings included:
    - When N bombs fall on N houses, approximately N/e houses survive (where e ~ 2.718).
    - The number 1/e (approximately 0.367 or 37%) emerged as the survival probability.
    - The maximum number of bombs hitting a single house increased logarithmically with the number of bombs.

5. Mathematical Connections: The discussion revealed deep connections between:
    - The compound interest formula and e.
    - Factorial functions and exponential series.
    - Taylor series expansion of e<sup>x</sup>.
    - Binomial probability distributions.
    - The relationship between these concepts and the bombing problem.

6. Practical Coding Exercises: Participants wrote Python code to simulate experiments and verify theoretical predictions. They computed factorials, ran simulations with different parameter, and observed convergence patterns.
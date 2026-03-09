---
layout: page
title: "08_Pandit_and_Pigeonhole - Discussion Summary"
permalink: /notes/08_pandit_and_pigeonhole/discussion_summary/
---

# Discussion Summaries : The Pandit and the Pigeonhole

## Summary - 1:

### Based on the meeting transcript, here are the key points of the discussion:

### 1. Pigeonhole Problem: The main topic was about a temple where a Pandit stores mobile phones in pigeonholes based on the last two digits of phone numbers (00-99). The discussion explored how phones would be distributed across these 100 pigeonholes.

### 2. Connection to Previous Bomb Problem: The pigeonhole problem was related to an earlier "bomb problem" involving houses. Both problems deal with random distribution and the mathematical constant e (approximately 2.718).

### 3. Key Observations About e:
- Approximately 37% (1/e) of pigeonholes remain empty.
- This 1/e ratio appears consistently across different random distribution problems.
- The group discussed why e appears in problems involving continuous, gradual processes.

### 4. Maximum Load Analysis:
- Using Python simulations, they found the maximum number of phones in any single pigeonhole rarely exceeds 6-8.
- The average maximum load was around 4.2.
- For n items, the maximum load appears to be approximately log(n).

### 5. Pattern Discovery: When visualizing the distribution, they noticed:
- Some pigeonholes consistently remain safer (less loaded).
- Gaps appear at regular intervals in the distribution.
- Corner positions tend to be safer.

### 6. Mathematical Relationships: The team explored probability calculations showing that (1 - 1/n)<sup>n</sup> converges to 1/e, connecting compound interest formulas to the distribution problem.

### 7. Open Questions: The group struggled to intuitively understand what e represents geometrically or conceptually, similar to how pi relates to circles.

---

## Summary - 2:

### This meeting was a detailed discussion focused on understanding probability distributions, optimization problems, and the mathematical constant e through several related problems - primarily the "temple phone storage problem" and the "bombing houses problem."

### Key Discussion Points:
1. Problem Statement: The main problem discussed was about a temple where visitors must deposit their phones in pigeonholes numbered 00-99, with phones stored based on the last two digits of their phone numbers. The team explored how many phones would accumulate in the busiest pigeonhole.

2. Connection to Previous Problems: The team recognized this problem was essentially identical to the earlier "bombing houses" problem - both involve random distribution across numbered slots (houses or pigeonholes).

3. Mathematical Observations:
- When running simulations with 100 houses/phones and 100 bombs/visitors, approximately 37% (1/e) of slots remain empty.
- The maximum load in any single slot tends to be around ln(n), where n is the number of slots.
- For 100 slots, maximum load is typically 4; for 1000 slots, it's around 6-7.

4. The Constant e:
- The team extensively discussed why e (approximately 2.718) appears in these probability problems.
- They explored the relationship: (1 - 1/n)<sup>n</sup> converges to 1/e as n increases.
- KG demonstrated that with different "kill rates" (probabilities), the pattern consistently converges to values related to e.
- The team concluded e appears in problems involving continuous, gradual processes and compounding effects.

5. Pattern Discovery: Through visualization experiments, the team discovered that "safe" houses (those receiving no bombs) appear at regular intervals in the distribution, suggesting underlying patterns in random distribution. (# this was later debunked #)

6. Key Formulas Derived:
- Number of survived houses after k rounds: n/e<sup>k</sup>.
- Bombs needed to destroy all houses: approximately n * ln(n).
- Maximum load in any slot: approximately ln(n).


### Philosophical Discussion: The team debated whether to understand e through mathematical formulas or intuitive reasoning, ultimately agreeing they needed to understand "what is e" fundamentally before fully grasping "why e appears" in these problems.

### The meeting ended with the team planning to further research the geometric and conceptual understanding of e (euler's number).
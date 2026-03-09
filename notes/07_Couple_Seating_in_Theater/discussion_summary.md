---
layout: page
title: "07_Couple_Seating_in_Theater - Discussion Summary"
permalink: /notes/07_couple_seating_in_theater/discussion_summary/
---

# Discussion Summaries : Couples Seating in Theater

## Summary - 1:

### The team analyzed a probability problem about couples randomly selecting seats in a theater, determining what fraction of seats remain empty when no more couples can be seated.

### Key Discussions:
### Problem Setup
- Couples arrive randomly and occupy two consecutive seats.
- Once seated, couples don't move.
- Theater stops admitting when only single isolated seats remain.
- Goal: Find the expected proportion of empty seats.

### Analytical Approach
### Simulation Results (JG's code):
- For n=10 seats: observed ~0.2 (20%) empty seats most frequently.
- For n=100 seats: converged to ~0.136 (13.6%) empty seats.
- Distribution skewed left: more probability near 0 than maximum.

### Theoretical Bounds:
- Minimum empty seats: 0 (best case all couples fit perfectly).
- Maximum empty seats: n/3 (worst case each couple leaves gaps).
- For n=100: maximum 34 empty seats, not 49 as initially thought.

### Mathematical Solution
### Probability Framework (led by ACP):
- Each couple fills 2 seats with probability 2/n.
- Probability of leaving empty: 1 - 2/n.
- After multiple trials: (1 - 2/n)<sup>(n/2)</sup>.
- Using limit: lim(n->inf) (1 - 1/k)<sup>k</sup> = 1/e.
- Substituting k = n/2: (1 - 2/n)<sup>(n/2)</sup> = 1/e<sup>2</sup>.

### Final Answer: 1/e<sup>2</sup> ~ 0.135 (13.5%)
This matches the simulation results, confirming the mathematical derivation.

### The team successfully derived that approximately 13.5% of theater seats remain empty in the asymptotic case through both simulation and rigorous mathematical proof.
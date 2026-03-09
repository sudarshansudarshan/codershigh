---
layout: page
title: "02_Lawyer_Revenue_Maximization - Discussion Summary"
permalink: /notes/02_lawyer_revenue_maximization/discussion_summary/
---

# Discussion Summaries : Greedy Lawyer and Profit Maximization

## Summary - 1:

### The meeting focuses on solving an optimization problem where a lawyer must maximize profit by selecting non-overlapping client appointments from multiple requests, with each appointment paying a fixed fee regardless of duration.

### Participants explore various algorithmic approaches including greedy methods based on start time, end time, duration, with several students proposing counter examples to disprove certain strategies while others use visual representations like calendars and tree diagrams to illustrate the complexity of the problem.

### The group converges on two promising approaches - sorting by earliest end time and sorting by shortest duration - but does not reach a definitive proof, with participants encouraged to continue testing these methods through coding and generating random test cases to validate their solutions.

### Next Steps:
- All participants: think through and find counter examples for the earliest end time approach to prove or disprove its optimality.
- Code a python program to generate random appointment slots and test different algorithms with exhaustive search for validation.
- Code and test the three approaches with sample data.
- All participants: do not search for solutions online or share spoilers from external sources to maintain the learning experience.

---

## Summary - 2:

### Note: this summary has been recorded for discussion 12 pm.

### The group continued their work on the lawyer scheduling optimization problem: maximizing profit by selecting the maximum number of non-overlapping appointments from 25 requests (9 AM - 6 PM window, $100 per appointment regardless of duration).

### Key Algorithms Tested:
1. Earliest End Time Algorithm (Forward Approach):
    1. Sort requests by end time, select earliest ending appointments.
    2. Eliminate conflicts after each selection.
    3. Result: 9 appointments (requests: 1, 4, 7, 10, 13, 16, 18, 22, 24) with Total duration of 392 minutes.
2. Latest Start Time Algorithm (Backward Approach):
    1. Work backward from 6 PM, select latest starting appointments.
    2. Result: 9 appointments (different selections).
    3. Total duration: 357 minutes.
3. Shortest Duration Algorithm:
    1. Previously tested, yielded only 7 appointments.
    2. Confirmed as suboptimal.

### Technical Progress:
- ACP and AB developed Python implementations using ChatGPT.
- Generated Gantt charts for visualization and used Google Colab for testing and validation.
- Manually verified non-overlapping schedules.

### Key Findings:
- Both forward and backward approaches achieved 9 appointments.
- Forward approach resulted in longer total working time (392 vs 357 minutes).
- Team believes both are logically equivalent but lacks formal proof.
- Different appointment selections but same count suggests multiple optimal solutions.

### Outstanding Questions:
- Are both approaches truly optimal?
- Which approach is better considering lawyer's rest time?
- Need mathematical proof of optimality.
- Require additional test datasets for validation.

### Next Steps:
- Generate new datasets for further testing.
- Implement reverse dataset testing.
- Continue seeking formal proof or counter-examples.

---

## Summary - 3:

### The team continued their discussion on the Greedy Lawyer problem. The goal is to maximize revenue by selecting non-overlapping appointments.

### Key Insights:
- Two main approaches were discussed: forward (earliest end time) and backward (latest start time).
- Gurudev provided a crutial hint: the appointment that ends first (A1) can always be included in the optimal solution without reducing the income (the number of appointments).
- The greedy algorithm approach: take the first ending task, discard all overlapping tasks, then repeat.

### The group is yet to discuss different varients of this problem:
1. Uniform fees according to appointment duration, with or without penalty for transition to different appointments.
2. Variable fees that is offered by the clients in the requests submitted on friday.
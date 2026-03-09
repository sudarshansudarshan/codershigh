---
layout: page
title: "04_Counting_Soldiers - Problem Statement"
permalink: /notes/04_counting_soldiers/problem_statement/
---

# Topic - 4 : Counting Soldiers / German Tank / Diya Placing

## Question:
### If you capture 10 random soldiers of an army with ID numbers, given that the ID numbers are serialized how do you estimate the total number of soldiers in the army?
### For example, if the 10 captured soldiers had numbers ranging from 109 to 8136, what's the total count of soldiers in the army?

---

## Additional Questions:
### Can we reverse this question? If we are given the population size, can we predict where the random soldiers will be given we pick N random soldiers?
### Can the question be changed to a scenario where we are observing random points on a line? If so, where will a random single point be estimated on a unit line over many experiments?
### What is this sense of fairness when we are picking things randomly?
### If we can estimate the positions of random points when we are given the population, can we estimate the population when we are given the random points?
### How will your estimation change if we increase or decrese the number of random points (sample size)?

---

## Coding Assignments:
### Create a program to find out where a particular random point will lie when we are generating N random points on a unit line.
### Plot the relationship between number of points and average distance between these points.
### Create programs to figure out the estimated minimum, estimated maximum, the populations size (range), and other things when we are given some N random points.
### Using the simulations and graphs try to come up with a formulas.
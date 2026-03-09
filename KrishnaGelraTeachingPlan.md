---
layout: page
title: Krishna Gelra Teaching Plan
permalink: /krishnagelrateachingplan/
---

# Teaching Plan — Coder's High S1 (Problems 1–10)

## Format (recommended)
- **10 sessions** (75–90 min each) OR **5 workshops** (2.5–3 hrs each)
- Session flow:
  1. Problem framing (10 min)
  2. Student attempts in groups (20 min)
  3. Guided solution paths (25 min)
  4. Edge cases + variants (15 min)
  5. Reflection + mini-assignment (10 min)

---

## Module A: Foundations of reasoning (Sessions 1–2)

### Session 1: GCD & Fibonacci (Problem 1)
**Learning goals**
- Euclid’s algorithm behavior
- Worst-case construction
- Recurrence intuition

**Activity**
- Compare step counts for random pairs vs Fibonacci pairs

**Assessment**
- Short proof: why consecutive Fibonacci numbers maximize Euclid steps

### Session 2: Pigeonhole methods (Problem 8)
**Learning goals**
- Guarantee arguments
- Constructive vs non-constructive proof

**Activity**
- Convert 3 daily scenarios into pigeonhole statements

**Assessment**
- 3 custom pigeonhole problems, increasing difficulty

---

## Module B: Optimization under uncertainty (Sessions 3–4)

### Session 3: Lawyer Revenue Maximization (Problem 2)
**Learning goals**
- Non-overlapping interval optimization
- Greedy vs DP intuition

**Activity**
- Solve with simple greedy; then find counterexample; then fix

**Assessment**
- Implement or hand-solve 6 test schedules

### Session 4: House/Job/Partner Hunting (Problem 5)
**Learning goals**
- Optimal stopping (secretary-style intuition)
- Threshold policies

**Activity**
- Simulate candidate streams and compare threshold strategies

**Assessment**
- Explain chosen stopping rule and expected success tradeoff

---

## Module C: Probability and estimation (Sessions 5–7)

### Session 5: Sniper Shooting (Problem 3)
**Learning goals**
- Geometric probability in circles
- Distance and area-based reasoning

**Activity**
- Monte Carlo sketch vs exact derivation

**Assessment**
- Derive probability for a modified radius/region setup

### Session 6: Dropping Golden Biscuits (Problem 6)
**Learning goals**
- Random spatial allocation and expected value
- Partitioning argument

**Activity**
- Model variants with weighted zones

**Assessment**
- Expected-value computation with changed distributions

### Session 7: Counting Soldiers (Problem 4)
**Learning goals**
- Population estimation from sampled labels
- Bias and uncertainty discussion

**Activity**
- Classroom mini “capture-recapture” simulation

**Assessment**
- Estimate + confidence narrative (conceptual)

---

## Module D: Combinatorics + geometry algorithms (Sessions 8–10)

### Session 8: Couple Seating in Theater (Problem 7)
**Learning goals**
- Occupancy/combinatorial counting
- Expected empty seats under constraints

**Activity**
- Enumerate small-n exactly, extrapolate pattern

**Assessment**
- Solve 2 variants with changed seat/couple rules

### Session 9: Bus Trip to Manali (Problem 9)
**Learning goals**
- Intuition-driven probability modeling
- Continuous/discrete approximation discussions

**Activity**
- Derivation alternatives: exact vs heuristic

**Assessment**
- Students present two different solution approaches

### Session 10: Closest Pearls on the Floor (Problem 10)
**Learning goals**
- Closest-pair concept and scaling bottlenecks
- Why brute force fails at scale

**Activity**
- Compare O(n^2) intuition with divide-and-conquer idea

**Assessment**
- Complexity comparison + pseudo-solution sketch

---

## Evaluation structure
- **20%** participation/discussion quality
- **30%** mini-assignment submissions (post-session)
- **20%** one group presentation (any 1 problem)
- **30%** final case-study challenge combining 2+ techniques

## Final capstone prompt (suggested)
Pick one real-world scenario and model it using:
1) a stopping/selection strategy, and
2) a probabilistic or combinatorial guarantee,
then justify assumptions and limitations.

## Instructor notes
- Keep emphasis on **reasoning clarity** over formula memorization
- Ask students to explain “why this model” before “what answer”
- Use quick simulations where exact derivation feels abstract

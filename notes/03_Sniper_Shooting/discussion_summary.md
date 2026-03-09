---
layout: page
title: "03_Sniper_Shooting - Discussion Summary"
permalink: /notes/03_sniper_shooting/discussion_summary/
---

# Discussion Summaries : Sniper Shooting / Dart Problem

## Summary - 1:

### Gurudev introduced a new problem: An archer shoots 100 times at a circular target (unit radius), with all shots landing inside the circle. The question asks for the expected distance from the center to the nearest shot.

### The group conducted extensive computational experiments:

### Multiple participants (SST, DC, ACP, KG) wrote Python code to simulate the problem.
- Two coordinate approaches emerged: Cartesian (x,y coordinates) and Polar (radius and angle).
- DC demonstrated that using polar coordinates (randomizing both radius and angle) properly captures the circular distribution.
- ACP ran comprehensive simulations varying two parameters: number of experiments and number of shots per experiment.

### Key Findings:
1. As the number of shots increases, the minimum distance to center decreases.
2. The relationship appears to follow an inverse square root pattern: distance is proportional to 1/√N where N is the number of shots.
3. At 10,000 shots, the distance was approximately 0.01, suggesting the formula might be close to 1/√N.
4. ACP performed curve fitting in Excel and confirmed the inverse square root relationship.

---

## Summary - 2:

### The problem: A shooter fires 100 shots at a circular target (radius 1 unit). None of the shots are perfect, i.e. they all land randomly within the circle. The goal is to find the expected minimum distance from the center across multiple experiments. In simple terms: what will be the estimated closest shot to the center if we throw 100 darts or shoot 100 bullets and all shots land inside the target area, but randomly?

### Key Findings:
- The team wrote code to simulate the experiment multiple times.
- They discovered the expected minimum distance follows the formula: approximately 1/√N, where N is the number of shots.
- When shots increased from 100 to 10,000, the minimum distance decreased from around 0.08 to 0.01.
- DC implemented using polar coordinates (random radius and random angle).
- The curve fitting showed the relationship is 0.9845/√X, very close to 1/√X.
- The value converges but keeps decreasing as more shots are taken (law of diminishing returns).

### The discussion involved heavy experimentation with Python code, data visualization, and mathematical analysis to understand this inverse square root relationship.

---

## Summary - 3:

### Main Problem: What is the expected distance from the center when randomly throwing a dart at a circular target?

### Key Discussions:
### 1. Random vs. Fair Selection:
- Random selection on a large scale equals fair selection.
- Random points divide data into equal parts on average.
- If bins are known, pick as many points as there are bins for fair sampling.

### 2. Why R and theta Don't Give Uniform Distribution:
- Simply picking random radius (r) and angle (0) clusters points near the center.
- Outer circles have more area, so they should receive proportionally more points.
- True randomness requires considering area, not just distance.

### 3. Two Proposed Answers Answers:
### Answer 1: 1/v2 ~ 0.707
- Derived by dividing circle into two equal areas.
- Inner circle area outer ring area.
- Mathematical formula: pi * r<sup>2</sup> =  pi * R<sup>2</sup> - pi * r<sup>2</sup>

### Answer 2: 2/3 ~ 0.667
- Suggested by simulation results.
- AB's triangle visualization using odd number sequence (1,3,5,7,9,11).
- Based on unrolling concentric circles into a triangle.

### 4. Generalization Proposed:
- For n darts: Expected minimum distance = 1/√(n+1).

### Unresolved Questions:
- Why do simulation and mathematical derivation give different results?
- Is the triangle transformation equivalent to the circle problem?
- Which answer (1/√2 or 2/3) is correct for single dart?

### Action Items:
- Everyone to write personal summaries.
- Every 7th day: collective summary discussion.
- Share handwritten derivations with instructor.

---

## Summary - 4:

### The meeting initially got disconnected by mistake, but everyone rejoined. The main focus was on solving a problem about finding the average distance of randomly thrown darts in a circle.

### Key developments:
### 1. Initial confusion: The team struggled with why directly randomizing R (radius) and theta doesn't give uniform distribution in a circle. HZ explained that area is proportional to R-squared, not R, so using uniform R creates bias toward the center.

### 2. Solution approach: The breakthrough came when the team realized they needed to divide the circle into equal areas (annular rings) rather than equal radius intervals. This ensures uniform probability distribution.

### 3. Mathematical derivation: Multiple approaches were discussed:
- JT proposed a weighted average method using circumference (2 * pi * R) as frequency weights.
- The team derived that the answer is 2R/3 for a circle of radius R.
- AB demonstrated using GeoGebra how equal area rings give equal probability.

### 4. Code verification: PK's simulation confirmed the 2/3 result by taking square root of uniformly distributed random numbers for radius.

### 5. Generalization: The team discovered a pattern for n - dimensional space, the expected distance is n/(n+1) times the radius. So 1D gives 1/2, 2D gives 2/3, 3D gives 3/4, etc.

### 6. Current status: The team successfully solved the problem both intuitively and computationally, understanding why equal area distribution is key - to uniform random point selection in circles, but is yet to derive a formula the complete solve the problem.

---

## Note: The problem is not yet completed and the team is yet to discuss upon this to get a better idea of this problem.
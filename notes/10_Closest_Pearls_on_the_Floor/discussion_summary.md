---
layout: page
title: "10_Closest_Pearls_on_the_Floor - Discussion Summary"
permalink: /notes/10_closest_pearls_on_the_floor/discussion_summary/
---

# Discussion Summaries : Closest Pearls on the Floor / Closest Pair of Points

## Summary - 1:
<!-- 17th Jan -->
### Detailed Meeting Summary: This was a technical problem-solving session lasting approximately 3+ hours with 25 participants, primarily focused on finding the closest pair of points in a 2D plane efficiently.

### Main Problem Discussion:
### 1. Initial Approach - Circle Growing Method (AB & Team):
- AB proposed a visualization approach where circles grow from random points until they collide.
- Each point starts with radius 0 and increases incrementally (0.1, 0.2, etc.).
- When two circles touch, those points are the closest pair.
- Collision detection logic was implemented similar to game mechanics.
- This approach was identified as having N-squared complexity.

### 2. Animation Implementation (Manimator):
- Manimator coded the solution using Manim library for visualization.
- Created 30 random dots in an 8x12 rectangle (from -6 to +6 on X-axis, -4 to +4 on Y-axis).
- Used radius 0.08 for display purposes only.
- The code performed brute force comparison with nested loops (lines 26-27).
- Calculated Euclidean distance between all point pairs.
- Tracked minimum distance found during iterations.
- Complexity confirmed as N-squared due to round-robin comparison of each point with every other point.

### 3. Algorithm Complexity Analysis:
The team explored various approaches and their complexities:
- Brute Force: O(N²) - comparing every point with every other point.
- K-Nearest Neighbor: Training complexity is O(D × N × log N).
- K-Means Clustering: O(N × K × D × T), but considered close to linear when K and D are small constants.
- Target: Achieve O(N) or at least better than O(N²).

### 4. Divide and Conquer Strategy (Main Solution Path):
The team developed a recursive partitioning approach:
1. Quadrant Division: Split the space using X and Y axes.
    - Left partition: all points with negative X coordinates.
    - Right partition: all points with positive X coordinates.
    - Could further divide into 4 quadrants (Q1, Q2, Q3, Q4).
2. Manhattan Distance Approach: "The Divine" proposed converting points to Manhattan distances (X + Y) and sorting them. The idea was to check consecutive points in the sorted list. However, ACP identified edge cases where points equidistant from origin might not be closest to each other, requiring restrictions to specific quadrants.
3. Complexity Analysis: The team analyzed that sorting would give O(n log n) complexity, which is better than the brute force O(n²) but not the target O(n) that was desired.
4. Excel Demonstration: ACP created a sample dataset with 24-25 random integer coordinate points, divided into quadrants. They calculated Manhattan distances within each quadrant, found pairs with zero difference, computed Euclidean distances for those pairs, and selected the minimum as the winner from each quadrant.
5. Boundary Edge Cases: The team recognized that closest points might lie across quadrant boundaries (like the India-Pakistan border analogy). They proposed checking only boundary points - creating a 3x3 grid around each point with epsilon distance, requiring only 8 neighbor comparisons per boundary point, maintaining linear complexity.
6. Recursive Partitioning Solution: "The Divine" and ACP converged on a recursive partitioning approach - similar to merge sort. The algorithm would:
    - Start with unit grid partitioning.
    - Identify cells with most points.
    - Recursively partition those cells (H/2 subdivisions).
    - Continue until cells have 2-3 points maximum.
    - For 1 point: compare with 8 neighbors.
    - For 2 points: trivial comparison.
    - For 3 points: only 3 comparisons needed.
    - Complexity Analysis:
        - The approach achieves O(N log N) complexity.
        - N/2 partitions are created for N points.
        - Each partition involves constant-time comparisons (8 neighbors maximum).
        - The number of partition levels is log N (similar to merge sort).
        - This is better than the brute force O(N²) approach.
        
    - The method is essentially a modified version of merge sort applied to geometric point data, where instead of sorting values, we're partitioning space and finding minimum distances while building back up the recursive tree.

---

## Summary - 2:
<!-- 19th Jan -->
### Main Problem Discussion: The team worked on the "Closest Pair Problem" - finding the two closest points from a set of random numbers in a one-dimensional space (a line) by scanning through the array only once, aiming for O(n) complexity instead of O(n log n) sorting approach.

### Key Concepts Explored:
1. Problem Setup: Given N random points on a line appearing in random order, find the two points with minimum distance without sorting.
2. Binning Strategy: The team discussed dividing the number line into bins of width delta (δ), where delta represents the current minimum distance. This approach was inspired by the "Pandit Problem" (pigeonhole principle) discussed in previous sessions.
3. Probability Questions: Two main probability questions emerged:
    - What is the probability that a new point falls between the current closest pair? (Answer: D/L, where D is the distance and L is the line length).
    - What is the probability that a new point forms a new closest pair? (Still being worked out: approximately 2ND/L).
4. Hashing/Dictionary Approach: Gurudev demonstrated using phone numbers as an example - taking last 3 digits to create 1000 bins for O(1) lookup time. This directly maps to the closest pair problem.
5. Vicinity Check: When a new point arrives, check points within ±1.5D distance (neighboring bins) to determine if it forms a closer pair.

### Technical Implementation:
- ACP worked on splitting numbers into bins and observed that some bins remain empty while others contain multiple numbers.
- The team discussed iterative splitting until bins contain manageable numbers of points.
- AB demonstrated a simulation approach using ChatGPT assistance.

### Pending Questions:
- Exact probability formula for new point disturbing closest pair.
- Optimal bin size selection.
- How many new points needed before observing a new closest pair.

### The session ended with plans to continue the probability calculations and algorithm refinement in the next meeting.

---

## Summary - 3:

### Meeting Summary:
### 1. Closest Pair Problem Visualization
**Interactive Simulation Development: SHS demonstrated a simulation showing points on a line (range 1-1000) with:**
- Green boundaries representing D-vicinity around each point.
- Real-time probability calculations as points are added.
- Ability to track which points disturbed the minimum distance.

**Key Observations:**
- Probability oscillation: Increases when points fall outside green zones, decreases when inside.
- Dense population effect: Impact of each additional point diminishes as more accumulate.
- Range independence: Gurudev proved changing range (1-100 vs 1-10000) doesn't affect fundamental disturbance patterns.

### 2. Refinements to Understanding
- "The Divine's" Insight: If a new closest pair forms but D doesn't decrease significantly (e.g., not less than D/2), probability may still increase.
- ACP's Statistical Concern: Single experiments aren't conclusive — Monte Carlo simulations needed across multiple trials.
- Gurudev's Correction: The real question is "What's the probability the k-th point disturbs?" analyzed across all possible orderings, not just one sequence. Formula 2/k represents this.

### 3. Coding Exercise: Probability Analysis
**Challenge:** Plot expected disturbances (Y-axis) vs. position K (X-axis) using 100 elements over 1 million iterations.

**Results:**
- Probability decreases as position increases (approximately 1/K pattern).
- Graph showed diminishing returns (like 1-e<sup>-x</sup>).
- Two competing factors: more points increase vulnerability zones, but decreasing D shrinks zones.

**Connection to Binning:** As K increases, disturbance probability stabilizes, suggesting optimal bin sizes for efficient algorithms.

### 4. Validating Probability Patterns Through Simulation
1. Experimental Methodology - Core Discussion \
ACP guided the team on proper experimental design:
    - Run 10,000+ iterations to eliminate statistical bias.
    - Generate random point sequences and track disturbances position-by-position.
    - Two measurement approaches:
        - Point-in-time: Probability that k-th element disturbs (0-1 value).
        - Cumulative: Average total disturbances up to position k.

2. Key Insight: Non-Monotonic Individual Runs
    - Animation showed probability fluctuates in single experiments.
    - True pattern emerges only through averaging many iterations.
    - Overall trend: probability decreases as more points added.

3. Simulation Results \
Multiple team members (JK, "The Divine", SHS, SHR) implemented and tested:
    - SHS's graph: Decreasing probability pattern (~0.66 for 2nd element, declining thereafter).
    - "The Divine"'s graph: Cumulative disturbances increase but at diminishing rate.
    - Pattern resembles 1/K or 2/K decay (harmonic series behavior).

4. Mathematical Understanding
    - Competing factors: More points create larger vulnerable regions (2D × n), but minimum distance D shrinks faster.
    - Rate of disturbance decreases even as total count increases.
    - Similar to diminishing returns and stochastic gradient descent convergence.

5. Connections to Previous Work
    - Related to empty bins experiment (~36% convergence).
    - Similar analytical approach to Fibonacci/GCD worst-case analysis.

**Outcome:** Successfully validated through simulation that disturbance probability follows predictable mathematical patterns, confirming the 1/K hypothesis.

---

## Summary - 4:

### Meeting Summary: Closest Pair Algorithm Discussion
<!-- Date: January 23-24, 2026
Duration: ~4 hours (starting 23:40:18)
Participants: Gurudev, ACP, "The Divine", "Daaku Mangal Singh", SHR, MM, AJ, SHS, AB, ASH, and others -->

### Key Topics Discussed:
**1. Randomized Closest Pair Problem:**
- Gurudev introduced a streaming algorithm for finding the closest pair of points using hashing and binning.
- Core concept: Use minimum distance (delta) as bin width to ensure closest pairs fall in same bin or adjacent bins.
- Probability of disturbance: 2/K for new points.
- Recommendation: Solve manually without GenAI to understand deeply.

**2. Hashing Approach Debate:**
- **Modulo vs. Division:** Extended discussion on whether to use modulo (remainder) or floor division (quotient) for hashing.
- **Modulo issue identified:** Can produce same hash key for numbers far apart (e.g., 64 and 91 both give remainder 1 when divided by 9).
- **Division approach:** Using quotient ensures consecutive keys for close numbers, avoiding false collisions.

**3. Algorithm Steps:**
- Start with first two numbers as champions (Ram and Lakshman).
- Calculate delta (minimum distance).
- Hash subsequent numbers using delta.
- Check same bin and left/right adjacent bins (maximum 3 comparisons).
- Rehash when new minimum distance found.
- Complexity: O(N) instead of O(N²).

**4. Implementation Challenges:**
- How to handle empty bins.
- Determining which neighboring bins to check.
- Ensuring no more than 2 elements per bin.
- Python type annotations discussion.

**5. Additional Topic Mentioned:**
- HyperLogLog algorithm for counting unique YouTube views (16 billion views example).
- Complexity: O(log log N) - "number of digits in number of digits".


### Implementing an optimized hashing algorithm for the closest pair problem:
**1. Algorithm Evolution**
- Started with modulo-based hashing approach.
- Switched to floor division after "The Divine" identified critical flaw.
- Floor division preserves spatial ordering on number line.
- Eliminates false collisions where distant numbers share bins.

**2. Core Algorithm Logic**
- Initialize delta with distance between first two points.
- Hash each new point using element // delta.
- Check only 3 adjacent bins (k-1, k, k+1) for proximity.
- When closer pair found: update delta and rehash all points.

**3. Complexity Analysis**
- Best case: O(n) with minimal rehashing.
- Worst case: O(n²) with frequent delta updates.
- Expected rehashes: ~2 log n operations.
- Significant improvement over naive O(n²) comparisons.

**4. Implementation Details**
- Dictionary structure: {bin_number: [list of values]}.
- Streaming data approach for one-by-one processing.
- Compared against brute force O(n log n) solution (~10ms for 1M points).

**5. Related Topics**
- YouTube views problem (O(log (log n)) space).
- Secretary problem and birthday paradox connections.
- Key Takeaway: Floor division creates spatially ordered bins, enabling efficient closest pair detection by checking only 3 adjacent bins per point.

**Outcomes:**
- Team agreed to continue working on implementation.
- Identified modulo hashing as problematic for this specific problem.
- Floor division approach proposed as better alternative.
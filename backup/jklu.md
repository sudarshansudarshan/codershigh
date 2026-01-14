---
layout: page
title: JOC @ JKLU
permalink: /jklu/
order: 2
---


# Joy of Computing Workshop - Class Notes

## Introduction

In today's workshop on the Joy of Computing, we explored a variety of intriguing topics that blend mathematics, computing, and real-world applications. The session covered:

- **Sudarshan's Inc Problem**: A game that challenges our understanding of averages and strategic investment.
- **Concept of Averages**: Case studies highlighting how averages can sometimes lead to paradoxical or counterintuitive conclusions.
- **Programming Puzzle**: Simulating the Sudarshan's Inc game to analyze potential profits or losses.
- **Additional Discussions**: Insights into auctions, CAPTCHA systems, and algorithmic recommendations on platforms like YouTube.

---

## 1. Sudarshan's Inc Problem

### Understanding the Game

**Sudarshan's Inc** offers a unique lottery game with the following rules:

- **Investment**: Participants invest any amount less than ₹50,000.
- **Winning Condition**: If your investment is above the average investment of all participants, you win.
- **Prize**: Winners receive a total of ₹50,000 (inclusive of their initial investment).
  - *Example*: If you invest ₹10,000 and win, you receive an additional ₹40,000.
- **Losing Condition**: If your investment is below the average, you lose your entire investment.

### Analyzing Sudarshan's Benefit

- **Revenue Generation**:
  - The company collects all investments from participants.
  - Only those above the average receive payouts.
- **Profit Mechanism**:
  - Since not everyone can be above average, there will always be losers whose investments contribute to the company's profit.
  - The company profits from the total investments of the losers minus the payouts to the winners.

---

## 2. The Concept of Averages

Averages are a fundamental statistical concept but can sometimes lead to unexpected interpretations.

### Case Studies

#### a. Migration and Average IQ

- **Scenario**: A group of people migrates from India to a neighboring country with a lower average IQ.
- **Outcome**:
  - **India**: The average IQ increases because lower-than-average individuals have left.
  - **Neighboring Country**: The average IQ also increases because the immigrants have a higher IQ than the country's average.
- **Explanation**: This paradox illustrates how averages can shift based on the movement of individuals relative to the mean.

#### b. The Optimistic Professor

- **Scenario**: A professor expects all students to score above the class average.
- **Reality Check**:
  - Mathematically impossible, as the average is calculated based on all scores.
  - Highlights a common misunderstanding of statistical averages.

#### c. The Fire and Ice Paradox

- **Scenario**: A person has their hair on fire and feet in ice water.
- **Average Feeling**:
  - On average, they might seem to feel neutral.
- **Reality**:
  - The person experiences extreme discomfort, demonstrating that averages can sometimes mask individual experiences.

### Discussion on Averages

- **Distribution Symmetry**:
  - In a perfectly symmetrical distribution, the number of values above and below the average is equal.
- **Implications in Sudarshan's Game**:
  - Not all participants can be above average; inevitably, some will lose.
  - Understanding this helps in strategizing investment amounts.

---

## 3. Programming Puzzle: Simulating Sudarshan's Inc Game

### Objective

- **Task**: Write a program to simulate 100 people playing Sudarshan's Inc game.
- **Goal**: Determine if Sudarshan's Inc profits or incurs a loss.

### Steps to Solve

#### a. Choosing a Distribution

- **Uniform Distribution**:
  - Every investment amount between ₹0 and ₹50,000 has an equal chance.
- **Normal (Gaussian) Distribution**:
  - Investment amounts cluster around a mean value with a certain standard deviation.

#### b. Simulating Investments

- **Generate Random Investments**:
  - Use a random number generator based on the chosen distribution.
  - Ensure all investments are less than ₹50,000.

#### c. Calculating the Average

- **Compute Average Investment**:
  - Sum all investments and divide by 100 (number of participants).

#### d. Determining Winners and Losers

- **Winners**:
  - Participants who invested above the average.
  - Each winner receives ₹50,000 total (including their investment).
- **Losers**:
  - Participants who invested below the average.
  - They lose their entire investment.

#### e. Calculating Profit or Loss

- **Total Payouts**:
  - ₹50,000 multiplied by the number of winners.
- **Total Investments Collected**:
  - Sum of all losers' investments.
- **Profit/Loss**:
  - Profit if total investments collected exceed total payouts.
  - Loss if total payouts exceed investments collected.

### Possible Outcomes

- **Profit Scenario**:
  - More participants invest below the average, leading to higher profits for Sudarshan's Inc.
- **Loss Scenario**:
  - Unlikely but possible if the distribution of investments is skewed.

---

## 4. Additional Discussions

### a. The Mobile Phone Auction (Vickrey's Model)

- **Auction Type**: Second-price sealed-bid auction.
- **Mechanism**:
  - Bidders submit sealed bids without knowing others' bids.
  - Highest bidder wins but pays the price of the second-highest bid.
- **Strategic Implications**:
  - Encourages truthful bidding, as overbidding doesn't increase the price paid unless another bid is close.
  - Reduces the winner's curse, where the winner overpays due to competition.

### b. The Human CAPTCHA Project

- **Purpose of CAPTCHAs**:
  - Distinguish between humans and bots.
  - Utilize human input to solve complex tasks.
- **Dual Tasks in CAPTCHAs**:
  - **Verification Task**: Ensures the user is human (e.g., typing distorted text).
  - **Data Collection Task**: Gathers data to train AI models (e.g., identifying objects in images).
- **Examples**:
  - Identifying zebra crossings helps improve self-driving car algorithms.
  - Transcribing blurred words aids in digitizing books.

### c. YouTube's Recommendation Algorithm

- **Algorithm Complexity**:
  - Analyzes user behavior to suggest relevant videos.
  - Factors include watch history, likes, shares, and session duration.
- **Creator Strategies**:
  - Content creators optimize videos to rank higher (e.g., clickbait titles, engaging thumbnails).
- **The Moving Target Phenomenon**:
  - As creators adapt to the algorithm, YouTube updates it to maintain content quality.
  - This continuous evolution prevents exploitation and enhances user experience.

---

# Joy of Computing Workshop - Afternoon Session

## Introduction

In the afternoon session of the Joy of Computing workshop, we delved into fascinating concepts that bridge social interactions, probability, and decision-making algorithms. The session covered:

- **Impression Network Data Collection**: An exercise in social networking and data analysis.
- **Markov Chains and Mood Switching**: Exploring state transitions and convergence through simulations.
- **The Online Hiring Problem**: Understanding optimal stopping theory and its real-world applications.

---

## 1. Impression Network Data Collection

### Activity Overview

We began with an interactive exercise designed to map social impressions within the classroom:

- **Task**: Each participant was asked to engage with others and note down the names of individuals they found impressive.
- **Objective**: To collect data that represents a network graph of students based on mutual impressions.

### Brainstorming and Analysis

We encouraged you to brainstorm and formulate deep questions about the collected data:

#### a. Potential Inferences

- **Identifying Influencers**: Who are the most frequently mentioned individuals?
- **Community Clusters**: Are there subgroups within the class where impressions are stronger?
- **Reciprocity**: Do impressions tend to be mutual?

#### b. Types of Analysis

- **Network Analysis**: Using graph theory to analyze connections.
  - **Degree Centrality**: Measuring the number of direct connections each individual has.
  - **Betweenness Centrality**: Identifying individuals who act as bridges between groups.
- **Sentiment Analysis**: If additional data is available (e.g., reasons for impressions), analyzing the sentiments behind them.
- **Visualization**: Creating network graphs to visually represent relationships.

#### c. Potential Business Ideas

- **Personalized Networking Platforms**: Creating apps that help people identify and connect with influential individuals.
- **Team Building Tools**: Assisting organizations in forming effective teams based on interpersonal impressions.
- **Marketing Strategies**: Leveraging influential individuals for product promotions within social networks.

---

## 2. Markov Chains and Mood Switching

### Introduction to Markov Chains

A **Markov chain** is a mathematical system that undergoes transitions from one state to another on a state space. It is characterized by being **memoryless**—the next state depends only on the current state and not on the sequence of events that preceded it.

### Two-State Markov Chain: Happy and Sad

#### a. Setting Up the Model

- **States**: Happy (H) and Sad (S).
- **Transition Probabilities**:
  - Probability of staying in the same state or switching to the other.
  - Represented in a **transition matrix**.

#### b. Excel Simulation

- **Initial Distribution**: An initial number of people in each state.
- **Iterations**:
  - Applied the transition probabilities to update the state distribution over several iterations.
- **Observation**:
  - The number of people in each state fluctuated initially.
  - After approximately 10 iterations, the distribution converged.

#### c. Convergence to Steady-State Distribution

- **Steady-State**: The state where the distribution remains constant over iterations.
- **Properties**:
  - Independent of the initial distribution.
  - Determined solely by the transition probabilities.
- **Mathematical Explanation**:
  - The steady-state distribution is the **eigenvector** associated with the eigenvalue 1 of the transition matrix.

### Three-State Markov Chain: Park, Apartment, Restaurant

#### a. Expanding the Model

- **States**: Park (P), Apartment (A), Restaurant (R).
- **Transition Matrix**:
  - A 3x3 matrix representing probabilities of moving between states.

#### b. Observations

- **Convergence**:
  - Similar to the two-state model, the system converged to a steady-state distribution.
- **Interpretation**:
  - Regardless of where people start, they eventually spend a predictable proportion of time in each location.

### Why Does Convergence Occur?

#### a. Role of Eigenvectors and Eigenvalues

- **Eigenvectors**:
  - Vectors that do not change direction under a linear transformation.
- **Eigenvalues**:
  - Scalars representing how the eigenvector is scaled during the transformation.
- **In Markov Chains**:
  - The steady-state distribution is the normalized eigenvector corresponding to the eigenvalue 1.

#### b. Mathematical Insight

- **Transition Matrix $$ T $$**:
  - Describes the probabilities of moving from one state to another.
- **Steady-State Condition**:
  - $$ T \cdot \pi = \pi $$ where $$ \pi $$ is the steady-state distribution.
- **Convergence**:
  - Due to the **Perron-Frobenius theorem**, which guarantees a unique largest eigenvalue (which is 1 for stochastic matrices) and a corresponding positive eigenvector.

### Connection to Hidden Markov Models

While we discussed Markov chains, it's important to distinguish them from **Hidden Markov Models (HMMs)**:

- **Markov Chains**:
  - The states are directly observable.
- **Hidden Markov Models**:
  - The states are not directly observable (hidden), but outputs dependent on the states are observable.
- **Applications**:
  - HMMs are widely used in fields like speech recognition, bioinformatics, and finance.

---

## 3. The Online Hiring Problem (Secretary Problem)

### Problem Description

You are faced with a sequence of options (e.g., job applicants, salaries, potential partners) that you must evaluate one at a time:

- **Objective**: Select the best (e.g., highest salary, most qualified applicant).
- **Constraints**:
  - You cannot return to a previous option once you have rejected it.
  - You must decide immediately after viewing each option whether to accept or reject it.

### Optimal Stopping Theory

This problem is a classic example of the **Optimal Stopping Theory** in probability and statistics.

#### a. The Strategy

- **Sampling Phase**:
  - **Reject** the first $$ n/e $$ candidates outright (where $$ n $$ is the total number of candidates and $$ e $$ is Euler's number, approximately 2.71828).
  - **Record** the highest value among the sampled candidates.
- **Selection Phase**:
  - **Accept** the first candidate who is better than all the candidates in the sampling phase.
- **Outcome**:
  - This strategy maximizes the probability of selecting the best candidate, with a success rate of about 37%.

#### b. Mathematical Justification

- **Optimal Threshold**:
  - The optimal number of candidates to sample is $$ k = n/e $$.
- **Probability of Success**:
  - The maximum probability of selecting the best candidate is $$ 1/e $$  (~36.8%).
- **Intuition**:
  - Balances the trade-off between gathering enough information and the risk of the best candidate appearing early.

### Application to the Salary Problem

#### a. Scenario

- **Goal**: Choose the job offer with the highest salary.
- **Process**:
  - Salaries are presented one by one in random order.
  - You must accept or reject each salary when presented.

#### b. Implementing the Strategy

1. **Sampling Phase**:
   - **Do not accept** any salary offers during the first $$ n/e $$ interviews.
   - **Keep track** of the highest salary seen so far.

2. **Selection Phase**:
   - **Accept** the first salary that exceeds the highest salary from the sampling phase.
   - If no salary exceeds this, accept the last one.

#### c. Outcomes

- **High Success Rate**:
  - This method ensures a high probability of selecting the highest or near-highest salary.
- **Risk Management**:
  - Reduces the chance of settling for a lower salary due to early acceptance.

### Real-World Applications

#### a. Dating and Marriage

- **Objective**: Find the best life partner.
- **Application**:
  - Date and evaluate a sample of potential partners without committing.
  - Commit to the next person who is better than all previous ones.

#### b. Hiring a Secretary

- **Objective**: Hire the most qualified candidate.
- **Application**:
  - Interview a portion of applicants without offering the job.
  - Hire the next applicant who surpasses the best from the initial interviews.

#### c. Apartment Hunting

- **Objective**: Rent the best available apartment.
- **Application**:
  - Visit a fraction of available apartments.
  - Choose the next one that is better than those already seen.

#### d. General Decision-Making

- **Optimal Stopping** is applicable in any scenario where decisions are sequential and irrevocable, and the goal is to maximize payoff.

---

# Markov Processes

Let's start by looking at a simple Markov process involving two states: Happy and Stressed.

![Markov Process with Two States: Happy and Stressed](/machinelearning/assets/images/markov1.png)

In the figure above, we have two states: Happy and Stressed.

Here’s what we know:
- 70% of people in the Happy state will become Stressed after some time (one iteration), while 30% will stay Happy.
- 50% of people in the Stressed state will become Happy after some time (one iteration), while 50% will stay Stressed.

Now, consider an initial scenario where there are 1000 people in the Happy state and 0 in the Stressed state. What will the distribution of people be after several iterations? Will it remain the same?

Let's try to do this for two iterations:

![Distribution After Two Iterations](/machinelearning/assets/images/markov2.png)
![Distribution After Two Iterations](/machinelearning/assets/images/markov3.png)
![Distribution After Two Iterations](/machinelearning/assets/images/markov4.png)

Do you notice how the distribution changes after two iterations?

Will it keep changing, or will it eventually stabilize?

Yes, it will converge after some time. But do you understand why?

To get a better understanding, you can write a program to see if this distribution converges over time. Here’s a simple code snippet to help you explore this:

```python
import numpy as np
A = np.array([[0.3, 0.5],[0.7, 0.5]]) # Transition matrix
v = np.array([1000, 0]) # Initial distribution
def iterate_until_convergence(A, v, tolerance=1e-6, max_iterations=10):
    for _ in range(max_iterations):
        v_next = A @ v
        if np.allclose(v, v_next, atol=tolerance):
            return v_next
        v = v_next
    return v
final_distribution = iterate_until_convergence(A, v)
total_population = np.sum(final_distribution)
percentage_distribution = final_distribution / total_population * 100
print(final_distribution, percentage_distribution)

```

Notice how the distribution changes with each iteration. Eventually, you'll see that it stops changing—it converges.

## Matrix Method

There's another way to approach this: through matrix operations.

Think of the probability of transitioning from one state to another as a matrix, and the initial distribution of people in both states as a vector.

Here's what the matrix looks like:

$$
\text{Transition Matrix: } M = 
\begin{pmatrix}
0.7 & 0.5 \\
0.3 & 0.5
\end{pmatrix}
$$

_Notice that the sum of the columns is 1._

And here’s the initial distribution vector:

$$
\text{Initial Vector: } v_0= 
\begin{pmatrix}
1000 \\
0
\end{pmatrix}
$$

Now, to predict the distribution after one iteration, you multiply the matrix with the vector:

$$
\text{New Distribution: } v_1 = 
\begin{pmatrix}
0.7 & 0.5 \\
0.3 & 0.5
\end{pmatrix}
\begin{pmatrix}
1000 \\
0
\end{pmatrix}
=
\begin{pmatrix}
700 \\
300
\end{pmatrix}
$$

So, to find the eventual distribution, would you keep performing matrix multiplications repeatedly?

![EVD](/machinelearning/assets/images/EVD1.png)

But do you realize that you don't need to do the matrix multiplication all the time? You just need to find $$M^{n}$$.

But $$M$$ is a matrix, so how easily can you compute $$M^{n}$$?

This is where EVD (Eigenvalue Decomposition) comes to our rescue! 

EVD, or Eigenvalue Decomposition, allows us to express the matrix $$M$$ in terms of its eigenvalues and eigenvectors.

We know that:

$$
A v = \lambda v
$$

where $$v$$ is the eigenvector and $$\lambda$$ is the corresponding eigenvalue.

![EVD](/machinelearning/assets/images/EVD2.png)

Multiplying a matrix by a vector $$v$$ $$n$$ times is equivalent to raising the matrix to the power $$n$$.

![EVD](/machinelearning/assets/images/EVD3.png)


Now, do you realize the importance and power of eigenvectors? They can be used to find any power of $$A$$ in no time.

Over time, this matrix multiplication will lead to a steady-state distribution, where further iterations will not change the result. This is the point of convergence.

So for the above example, we get the final distribution to be:

$$
\begin{bmatrix}
416.666368 \\
583.333632
\end{bmatrix}
$$

**Derivation for convergence in Markov Matrix**

![Markov Convergence Derivation](/machinelearning/assets/images/markovder1.png)
![Markov Convergence Derivation](/machinelearning/assets/images/markovder2.png)


---

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

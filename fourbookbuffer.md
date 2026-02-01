---
layout: page
title: The 4-Book Buffer Puzzle
order: 7
permalink: /fourbookbuffer/
---

## The Puzzle

You need to get **100 books** home from the library, at the rate of **one new book every week**.

- The books you ultimately need are in a known sequence:  
  $$b_1, b_2, b_3, \ldots, b_{100}$$

- At any time, you can hold **only 4 books**.  
  Let the books currently with you be:  
  $$z_1, z_2, z_3, z_4$$

Each week:

1. You go to the library and receive the next required book in the sequence.
2. Since you can carry only 4 books, you must **give up exactly one** of the 4 books you currently have, to make space for the new one.

So, if your current holding is  
$$\{z_1, z_2, z_3, z_4\}$$  
and the next required book is $$b_k$$, then after the swap your holding becomes:  
(remove one of $$z_1, z_2, z_3, z_4$$ and add $$b_k$$).

---

## The Core Question

By the time you are about to bring home the final book $$b_{100}$$:

1. **Which book will you give up** (from your current four) to make room for $$b_{100}$$?
2. In the **next week**, you again receive the next book in the sequence (assume the sequence conceptually continues beyond 100), and must give up one of your four again:
   - **Which book will you give up next week?**
3. And in the weeks after that:
   - **What is your strategy for deciding which book to give up each time?**

---

## What You Know

- You know the entire required sequence in advance:  
  $$b_1, b_2, \ldots, b_{100}$$
- You always receive the next book in order.
- You always have exactly four books in hand.
- You must decide which one to drop each week.

---

## Your Task

Give a clear strategy (or rule) that determines, for each week:

- which book among  
  $$z_1, z_2, z_3, z_4$$  
  should be given up, so that you can proceed through the sequence as efficiently as possible—especially answering:

- which book you drop when bringing in $$b_{100}$$, and  
- what you drop in the subsequent week, and the weeks after that.
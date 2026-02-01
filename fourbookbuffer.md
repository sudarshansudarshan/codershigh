---
layout: page
title: The 4-Book Buffer Puzzle
order: 7
permalink: /fourbookbuffer/
---

## The Puzzle

You need to get **100 reference books** home from the library, at the rate of **one book per week**.

- The books you need follow a known sequence:  
  $$b_1, b_2, b_3, \ldots, b_{100}$$  

  The sequence may contain **repetitions**. That is, the same book may appear multiple times in the sequence.

- At any time, you can hold **only 4 books**.  
  Let the books currently with you be:  
  $$z_1, z_2, z_3, z_4$$

Each week:

1. You need the next book in the sequence, $$b_k$$.
2. If $$b_k$$ is already among the books you have, you **do not visit the library** that week.
3. If $$b_k$$ is **not** among the books you have, you must visit the library to get it.
4. Since you can carry only 4 books, if you already have 4 books with you, you must **give up exactly one** of them to make space for $$b_k$$.

So, if your current holding is  
$$\{z_1, z_2, z_3, z_4\}$$  
and the next required book is $$b_k$$ (which you do not already have), then after the visit your holding becomes:  
(remove one of $$z_1, z_2, z_3, z_4$$ and add $$b_k$$).



## The Objective

Your goal is to **minimize the total number of visits to the library** over the 100 weeks.



## The Core Question

By the time you are about to bring home the final book $$b_{100}$$:

1. **Which book will you give up** (from your current four) to make room for $$b_{100}$$, if a visit is required?
2. In the **next week**, you again need the next book in the sequence (think of the sequence as conceptually continuing beyond 100), and must decide again:
   - **Which book will you give up next week, if required?**
3. More generally:
   - **What is your strategy for deciding which book to give up each time you are forced to visit the library?**



## What You Know

- You know the entire required sequence in advance:  
  $$b_1, b_2, \ldots, b_{100}$$
- Books may repeat in the sequence.
- You only visit the library if the required book is not already with you.
- You always have at most four books in hand.
- Whenever you visit and already have four books, you must drop exactly one.



## Your Task

Give a clear strategy (or rule) that determines, for each week in which a visit is required:

- which book among  
  $$z_1, z_2, z_3, z_4$$  
  should be given up,

so that the **total number of library visits is as small as possible**, especially addressing:

- which book you drop when bringing in $$b_{100}$$, and  
- what you drop in the subsequent week, and the weeks after that.
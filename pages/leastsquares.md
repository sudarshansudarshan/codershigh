---
layout: page
title:  Let us Understand the Least Understood, Fair and Square!
order: 5
permalink: /leastsquares/
---

1. We encounter equations very often in our lives. Consider for example, the following situation at ___Baker's Cafe___. The manager has a very important estimate to make. Mostly, visitors at his cafe happen to be families and they are often comprised of Children and/or Adults. He observes that there are 3 adults and 1 child at a table and their bill turns out to be Rs.1200/-. There is yet another table with 2 children and 1 adult and their bill comes out to be Rs.1000/-. Can the manager estimate the consumption of a Child/Adult? This is popularly called the _Simultaneous Equations_ and we all remember from our school days, multiple ways in which these can be solved.<br>
$$ 3A + 1C = 1200 $$   
$$ 1A + 2C = 1000 $$

2. While we were taught the so called two variables and two unknowns, what if there were more equations than unknowns?<br>
$$ 3A + 1C = 1200 $$   
$$ 1A + 2C = 1000 $$    
$$ 1A + 1C =  900 $$


3. Note that the previous question can be modelled as a matrix:

   $$ 3A + 1C = 1200 $$   
   $$ 1A + 2C = 1000 $$    
   $$ 1A + 1C =  900 $$

   <u>Observe</u> this is same as :

   $$ \left( \begin{matrix} 3 & 1 \\1 & 2 \\1 & 1 \\\end{matrix}\right) $$
   $$\left(
   \begin{matrix}
   B\\
   C\\
   \end{matrix}
   \right)$$
   =
   $$
   \left(
	\begin{matrix}
	1200\\
	1000\\
	900\\
	\end{matrix}
   \right)
   $$

4. The best way to solve is, is to guess the values :-). Can you write a python code to guess the values?

5. How do you solve this mathematically? There are two nice ways of solving this:   
 - Model this as a question of inverting a rectangular matrix and find the solution. (Whoa! my teacher never taught me that!) 
 - Model this as a funtion of two variables and solve it using partial differentiation (Eeks!)
 
    



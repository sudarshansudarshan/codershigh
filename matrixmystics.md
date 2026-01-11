---
layout: page
title: Matrix Mystics
order: 5
permalink: /matrixmystics/
---

* TOC
{:toc}
# Module 1


___

1. Ram and Lakshman were two brothers, Ram's pocket money was twice as much as Lakshman. The good boy that Ram and Lakshman were, they did not spend their pocket money on anything. They instead saved the same in their piggy bank. Every week, they would check their savings so far. Assume the first week's savings was $$(R_1,L_1)$$ and second week's $$(R_2,L_2)$$ and so on. They try plotting their weekly savings on a graph sheet. How will the points look like?

2. Atul's house is centered at origin $$(0,0)$$ he walks straight (along the x-axis) for 2 units and then takes a left and walks 1 unit to reach Bala's house, after that he takes a right turn and walks for one unit and then a left turn and walks for one unit and reaches Chetan's house. He continues in a similar style, takes a right turn 1 unit and then left turn one unit and reaches Divya's house. Are the houses of Bala, Chetan and Divya on a straight line? What is the equation of this line? Plot this on Geogebra



3. Plot the lines $$y=x$$, $$y=2x$$, $$y=10x$$.

4. Observe that they all pass through the origin. Why?

5. Plot $$y=2x+1$$. Observe, Why doesn't it pass through the origin?

6. Plot $$y=ax+b$$, with $$a$$ and $$b$$ as parameters which you should be able to vary. What do you observe?

7. Consider the following simultaneous equation:

   $$2x+3y=7$$ <br>
   $$3x+4y=10$$ <br>

   Do you see a 2x2 matrix here? What is the importance of seeing a matrix in this problem? Why study matrices in general?<br>Do you observe that this problem can be retold as: <br>$$ \left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) $$
   $$\left(
   \begin{matrix}
   x\\
   y\\
   \end{matrix}
   \right)$$
   =$$\left(
   \begin{matrix}
   7\\
   10\\
   \end{matrix}
   \right)$$
8. Consider a simple function $$f(x) = 3x+2$$. This function is invertible right? Can you tell us what is $$\alpha$$ such that $$f(\alpha)=17$$? Is such an $$\alpha$$ unique? How did you find such an $$\alpha?$$. Is this always possible?

9. Consider the function $$f(x)=x^2-10$$, what is $$f(5)$$?

10. Consider the function $$f(x)=x^2-10$$, if $$f(\alpha)=54$$, what is $$\alpha$$?

11. Consider the function $$g(x)=x^3-x^2-10x+2$$, if $$g(x)=-22$$ what is $$x$$?


12. Do you know what is $$\mathbb{R}, \mathbb{R}^2 and\ \mathbb{R}^3$$ ? 


13. Consider the function $$\phi : \mathbb{R}^2\rightarrow \mathbb{R}^2$$ defined by $$\phi (x,y)=(2x+3y,3x+4y)$$. What has this to do with the previous question?

14. Is the function $$\phi$$ invertible? In the question above on matrices, we see that it is of the form $$A\vec{x}=b$$. Note that we can invert the matrix, using the method that was taught to us in our high school to find out the value for the variables $$x$$ and $$y$$. This is one of the many applications of matrices.

15. We will now see matrices as functions. Instead of $$\phi$$ we will write the matrix itself: <br>$$\left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$. 

16. Consider the function $$\left( \begin{matrix} 1 & 2 \\2 & 4 \\\end{matrix}\right) : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$. This matrix takes a few elements to the origin. What are those elements? Plot this using Geogebra.



# Module 2

---

1. $$A$$ is assigned $$0$$, $$B:1$$, $$C:2$$, and so on up to $$Z:25$$<br>
Assume you denoted every letter with a number, as given in the table above.<br> You need to encrypt the word $$SUDARSHANA$$ which stands for the numbers: $$18, 20, 3, 0, 17, 18, 7, 0, 13,0$$. <br>
You encrypt this using a matrix given by : $$ \left( \begin{matrix} 2 & 3 \\3 & 4 \\\end{matrix}\right) $$. <br>
So $$SUDARSHANA$$ will end up becoming: $$96, 134, 6, 9, 88, 123, 14, 21, 26, 39$$. <br>
Given these numbers, how will you decrypt the message and get back $$SUDARSHANA$$?<br>. This is a well known cryptographic protocol called the Hill Cipher. You can read more online.
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
   A\\
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



4. One obvious way to solve this, is to guess the values :-). Can you get closer to the solution by guessing? Note that there is no solution to this question. You can just reduce the error. Do you see why?

5. In the figure below:
![fig1](/codershigh/assets/markov2.png)
If 1000 people were to start in one state, what will be the distribution of people eventually?

5. In the figure below:
![fig2](/codershigh/assets/markov3.png)
If 1000 people were to start in one state, what will be the distribution of people eventually?

# Module 3

___

1. Use Geogebra:
Draw the vector $$\begin{bmatrix}1 \\
1 \\
\end{bmatrix}$$. Find out all those vectors which are perpendicular to this vector.

2. Do you observe that we are asking for vectors $$\begin{bmatrix}x \\
y \\
\end{bmatrix}$$ such that,
$$\begin{bmatrix}1 & 1 \\
\end{bmatrix}  \begin{bmatrix} x\\ y \\ \end{bmatrix}=0 $$

3. Use Geogebra and solve the above question with $$\begin{bmatrix}   1 \\
1 \\
\end{bmatrix}$$ replaced by $$\begin{bmatrix}a \\
b \\
\end{bmatrix}$$.Use $$(a,b)$$ as parameters and check what happens to $$(x,y)$$.

4. What is $$(x,y,z)$$ satisfying the following equation? (Use Geogebra)
$$\begin{bmatrix}1 & 2 & 3\\
\end{bmatrix}  \begin{bmatrix} x\\ y \\ z\\ \end{bmatrix}=0 $$

5. Use Geogebra and plot all the points in the set below.
$$T= \{ \alpha(1,2,1) | \alpha \in \mathbb{R}\} $$

6. Use Geogebra and plot all the points in the set below.
$$S= \{ \beta(2,7,3) | \beta \in \mathbb{R}\} $$

7. Use Geogebra and plot all the points in the set below.
$$W= \{\alpha(1,2,1) + \beta(2,7,3) | \alpha,\beta \in \mathbb{R}\} $$

8. In the above set $$W$$ find out all the points $$(x,y,z)$$ satisfying the following: (Use Geogebra)
$$\begin{bmatrix}w_1 & w_2 & w_3\\
\end{bmatrix}  \begin{bmatrix} x\\ y \\ z\\ \end{bmatrix}=0 $$
 where $$(w_1,w_2,w_3) \in W$$. Note that $$w_i$$s are real numbers.

9. Given the matrix $$A=\begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix}$$, find out all the possible $$(x,y,z)$$ such that:
$$ \begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix} \begin{bmatrix} x\\ y\\ z\\ \end{bmatrix}=0$$
 Observe carefully, what has this question got to do with previous five questions in this module

10. Given the matrix $$A=\begin{bmatrix}1 & 2 & 3\\ 4 & 5 &6\\ 7 & 8 & 9\\ \end{bmatrix}$$ what does the following three sets represent?<br>
(i) $$\mathscr{R}=\{\alpha(1,2,3) + \beta(4,5,6) + \gamma(7,8,9) |\alpha, \beta, \gamma\in \mathbb{R}\} $$<br>
(ii) $$C=\{\alpha(1,4,7) + \beta(2,5,8) + \gamma(3,6,9) | \alpha, \beta, \gamma \in \mathbb{R}\}$$<br>
(iii) $$N=\{(x,y,z)|x(1,4,7) + y(2,5,8) + z(3,6,9) = 0 \}$$<br>
 Use only Geogebra :)

11. Did you observe that every vector of $$\mathscr{R}$$ is perpendicular to every vector of $$N$$?

12. Consider the matrix $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}$$. Draw the line $$2y+x=4$$. Seeing the matrix $$B$$ as a function $$B:\mathbb{R^2}\mapsto \mathbb{R^2}$$,<br> where does $$B$$ takes the line  $$2y+x=4$$?<br>
Where does it take:<br>
i)$$2y+x=10$$<br>
ii)$$2y+x=62$$<br>
iii)$$2y+x=1800$$

13. In general $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}:\mathbb{R^2}\mapsto \mathbb{R^2}$$, where does this function take $$2y+x=k$$?(where $$k$$ is a constant)

14. Given $$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}:\mathbb{R^2}\mapsto \mathbb{R^2}$$. What is the range of this function?

15. You have achieved the required wisdom if you have realized that: <br>
$$B=\begin{bmatrix} 1 & 2 \\ 2 & 4\\ \end{bmatrix}:\mathbb{R^2}\mapsto \mathbb{R^2}$$. <br>
" $$B$$ collapses a dimension ".<br>

# Module 4

1. Given the matrix $$M=\begin{bmatrix} 1 & 3 \\ 2 & 6\\ \end{bmatrix}$$. Use Geogebra to plot $$\mathscr{R}$$, $$\mathscr{C}$$ & $$\mathscr{N}$$. what do you observe?<br>
(i) $$\mathscr{R}=\{\alpha(1,3) + \beta(2,6) | \alpha, \beta\in \mathbb{R}\} $$<br>
(ii) $$\mathscr{C}=\{\alpha(1,2) + \beta(3,6) | \alpha, \beta\in \mathbb{R}\} $$<br>
(iii) $$\mathscr{N}=\{(x,y)| x(1,3) + y(2,6) = 0, \forall x,y\in \mathbb{R} \}$$<br>

2. Note that $$\mathscr{R}$$ and $$\mathscr{N}$$ are orthogonal.<br>

3. What is  the null-space of $$M=\begin{bmatrix} 1 & 3 \\ 2 & 6\\ \end{bmatrix}$$ & the null-space of $$M^T$$?<br>

4. Do you observe that $$C(M)$$ &#x22A5; $$N(M^T)$$ , &nbsp; $$R(M)$$ &#x22A5; $$N(M)$$ ?<br>

5. Consider $$A=\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \\ \end{bmatrix}$$. What is $$N(A)$$, $$C(A)$$, $$R(A)$$, $$N(A^T)$$.<br>

6. Consider a 4x4 matrix $$M$$: $$\mathbb{R^4}\mapsto \mathbb{R^4}$$ whose range is<br>
a) $$4-Dimension$$<br>
b) $$3-Dimension$$ <br>
c) $$2-Dimension$$ <br>
d) $$1-Dimension$$ <br>
e) $$0-Dimension$$ <br>
Give an example each for all the above 5 cases.<br>

7. Consider $$A : \mathbb{R^{3}} \to \mathbb{R^{3}} $$<br>
a) Show that if the range contains a point $$(a,b,c)$$, then it should contain the entire set $$S$$, defined by:
$$S= \{\alpha(a, b,c)| \alpha \in \mathbb{R}\}$$. <br>
b) Show that if the range contains the points $$(a,b,c)$$ and $$(d,e,f)$$, then the range contains the entire set $$T$$ defined by:
$$T=\{\alpha(a,b,c) + \beta(d,e,f) \thinspace|\thinspace  \alpha,\beta\in \mathbb{R}\}$$.<br>
c) Note: $$S$$ is of the dimension $$1$$, but $$T$$ need'nt be of dimension $$2$$. Think! 

# Module 5

1. Give an example of two  $$2-dim$$ subspaces in $$\mathbb{R^{3}}$$. Let us call it $$S_1, S_2$$.


2. Let $$S_3$$ be all those vectors perpendicular to $$S_1$$. $$S_4$$ be that of $$S_2$$.


3. Find a matrix $$M$$ whose Null-Space is $$S_3$$. column space is $$S_2$$.


4. What does $$S_1$$ and $$S_4$$ represent?

5. Do you observe there is a bijection from $$S_1  \to S_2$$?

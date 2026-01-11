---
layout: page
title: Oceanverse 
order: 5
permalink: /linalg75/
---

* TOC
{:toc}


# Linear Algebra

1. Consider the matrix 
   $$
   \left[ \begin{array}{cc}
   1 & 2\\ 3 & 4
   \end{array}\right]
   $$
   - What does it remind you of? 
   - What does it denote? 
   - Where and why do we use a matrix? 
   - Can you enlist a few applications of matrices?    
   <br>  

2. Define a function. What is a surjective, injective and bijective
   function?

3. Give an example of a function
   $$
   f:\mathbb{R}^2\rightarrow\mathbb{R}^2
   $$

4. Give an example of a very nice function
   $$f:\mathbb{R}^2\rightarrow\mathbb{R}^2$$
   - Make extra efforts to make this function really nice. 
   - Explain what is so nice about your
     function? 
   - Why should one study such functions?   
   <br>
5. Define a function 
   $$ \phi : \mathbb{R}^2 \rightarrow \mathbb{R}^2 $$, which satisfies the following property: The point $$ \phi(2,3)=(7,4) $$. Note that this function should be defined at all points on $$\mathbb{R}^2$$. 
   - What are the properties of your function? Observe it
   microscopically.   
   <br>
   
6. Given a function $$\phi : \mathbb{R}^2 \rightarrow \mathbb{R}^2$$
   which satisfies the following two conditions:

   $$\phi(u+v)=\phi(u) +\phi(v)$$

   $$\phi(\alpha v)=\alpha\phi(v)$$

   where $$u=( x_{1} , y_{1} )$$, $$v=( x_{2} , y_{2} )$$ and $$u,v \in \mathbb{R}^2$$

   * What can one say of such functions? 
   * Observe this function closely, such functions form the crux of several discplines, mainly of sciences and engineering. Spend at least 20 minutes dissecting them to the best possible extent.  
   <br>
8. Consider $$\mathbb{R}^2$$ what are all the properties of this set?
   $$\mathbb{R}^2$$ is called a space of all vectors, aka a vector space.
   Lookup for the definition of a vector space.

9. A subset of a vector space which in itself is a vector space is
   caled a subspace. Give an example of a subspace of $$\mathbb{R}^2$$.

10. Given a vector $$(1,7)$$, what does the set
   $$\{ \alpha(1,7) | \alpha \in \mathbb{R}\}$$ represent? Is it a
   subspace of $$\mathbb{R}^2$$?

11. Is $$\mathbb{R}^3$$ a vector space?

12. Conside the two points $$(1,2,3)$$ and $$(4,5,7)\in \mathbb{R}^3$$. What
    does the following set denote:
    $$\{\alpha(1,2,3)+\beta(4,5,7) | \alpha, \beta \in \mathbb{R}\}$$.
    Is this a subspace?

13. Consider a straight line $$y=2x+1$$ in $$\mathbb{R}^2$$, does it form a
    subspace of $$\mathbb{R}^2$$?

14. Consider a unit circle in $$\mathbb{R}^2$$, centered at origin, is it
    a subspace of $$\mathbb{R}^2$$?

15. What are all the subspaces of $$\mathbb{R}^2$$?

16. What are all the subspaces of $$\mathbb{R}^3$$?

17. Given $$\mathbb{R}^3$$, pick any two points $$u,v\in \mathbb{R}^3$$.
    Note that $$\{\alpha u+\beta v | \alpha, \beta \in \mathbb{R}\}$$ is a
    subspace of $$\mathbb{R}^3$$. Generalize this idea!

18. The set $$\{\alpha \vec{u} + \beta \vec{v} | \alpha, \beta \in \mathbb{R}\}$$ is
    called the linear combination of vectors $$\vec{u}$$ and $$\vec{v}$$. We can
    generalize this to $$k$$ vectors. Observe what this set is all about?

19. We say that a vector $$\vec{w}$$ is manufactured by $$\vec{u}$$ and $$\vec{v}$$ if
    $$w\in \{\alpha \vec{u} +\beta \vec{v} | \alpha, \beta \in \mathbb{R} \}$$.

20. Show that $$(1,2,3)$$ and $$(4,5,6)$$ can manufacture $$(7,8,9)$$. Also
    $$(4,5,6)$$ and $$(7,8,9)$$ can manufacture $$(1,2,3)$$. Finally $$(4,5,6)$$
    can be manufactured by the other two vectors.

21. Can $$(2,1,0)$$ and $$(3,0,8)$$ manufacture $$(1,1,1)$$ ?

22. Can $$(0,0,1)$$ and $$(0,1,0)$$ manufacture $$(1,0,0)$$?

23. When can two vectors in $$\mathbb{R}^3$$ manufacture a given third
    vector?

24. When can two vectors in $$\mathbb{R}^3$$ fail to manufacture a given
    third vector?

25. If $$\{\vec{u},\vec{v},\vec{w}\}$$ are such that a vector in this set can be
    manufactured by some vectors in the same set, then such a set is
    called a linearly dependent set.

26. Give examples of a linearly dependent set in $$\mathbb{R}^3$$ and get
    conversant with the definition.

27. If $$\{\vec{u},\vec{v},\vec{w}\}$$ are such that no vector in this set can be
    manufactured by any combination of vectors in the same set, then such
    a set is called a linearly independent set.

28. Give examples of a linearly dependent set in $$\mathbb{R}^3$$ and
    $$\mathbb{R}^2$$ and get conversant with the definition.

29. Are $$(1,2), (3,4)$$ linearly independent in $$\mathbb{R}^2$$? Prove!

30. Are $$(1,1),(2,3),(7,17)$$ Linearly Independent or Dependent?

31. - Construct a set of 3 vectors that are Linearly Independent in
    $$\mathbb{R}^2$$. Can you?

    - Construct a set of 3 vectors that are Linearly Independent in
    $$\mathbb{R}^3$$. Can you?

    - Construct a set of $$k$$ vectors that are Linearly Independent in
    $$\mathbb{R}^k$$. Can you?

    - Construct a set of $$k+1$$ vectors that are Linearly Independent in
    $$\mathbb{R}^k$$. Can you?

32. - Show that in $$\mathbb{R}^2$$ we can at most have 2 Linearly
    Independent vectors.

    - Show that in $$\mathbb{R}^3$$ we can at most have 3 Linearly
    Independent vectors.

    - Show that in $$\mathbb{R}^n$$ we can at most have $$n$$ Linearly
    Independent vectors.

33. Set of any two linearly independent vectors in $$\mathbb{R}^2$$ is
    called a basis. Set of any three linearly independent vectors in
    $$\mathbb{R}^3$$ is called a basis. Similarly, for $$n$$.

34. Show that a basis can manufacture any vector of the vector
    space.

35. Show that any set of linearly independent vectors form a subset of
    some basis. In other words, one can include a few more elements to a
    linearly independent set and make it a basis.

36. Show that the number of elements in any basis for a given vector
    space is always constant.

37. Try taking a few vectors in $$\mathbb{R}^3$$ and discuss its linear
    independence or linear dependence. Try atleast 10 examples and
    familiarize yourself.

38. Show that any 3 vectors on a plane passing through the origin in
    $$\mathbb{R}^3$$ cannot be linearly independent. Prove.

39. What are all the subspaces of $$R^3$$.

40. Consider a subspace of $$R^3$$ and write down its basis. Do this for 3
    to 4 different subspaces.

41. Give an example of a function
    $$f:\mathbb{R}^2 \rightarrow \mathbb{R}^2$$ such that the range of the
    function is the straight line $$y=10x$$.

42. As an example consider the following basis set of
    $$\mathbb{R}^2 : \left \{(1,2),(2,2)\right \}$$. Construct a function
    $$\phi:\mathbb{R}^2\rightarrow \mathbb{R}^2$$ such that:

    $$\phi(\vec{u}+\vec{v})=\phi(\vec{u})+\phi(\vec{v})$$

    $$\phi(\alpha \vec{u})= \alpha \phi(\vec{u})$$

    Such a function is called a LT function,

    -  Where is (1,2) and (2,2) mapped?

    -  Where is (1,0) and (0,1) mapped?

    -  What is the range of this function?

43. Consider a function $$\phi$$ which is LT which maps

    $$\phi(1,2)=(3,4)$$

    $$\phi(6,6)= (2,0)$$

    -  How many such functions can you construct?

    -  What is the range of this function?

44. Discuss the range of the following functions, given their values at
    a few points:

    $$\phi(1,2)=(3,4)$$ $$\&$$ $$\phi(1,1)=(6,8)$$

    $$\phi(1,1)=(2,2)$$ $$\&$$ $$\phi(3,3)=(4,4)$$

    $$\phi(1,2)=(3,5)$$ $$\&$$ $$\phi(0,8)=(3,0)$$

    $$\phi(-2,2)=(0,0)$$ $$\&$$ $$\phi(8,2)=(1,1)$$

    $$\phi(1,1)=(2,2)$$ $$\&$$ $$\phi(1,2)=(3,3)$$

45. Give an example of an LT function which maps a L.I. set of vectors
    to a L.I. set of vectors i.e.
    $$\phi:\mathbb{R}^2 \rightarrow \mathbb{R}^2$$, where
    $$\left \{ \vec{u},\vec{v} \right \}$$ are L.I. $$\&$$
    $$\left \{\phi(\vec{u}), \phi(\vec{v})\right \}$$ are also L.I.

46. Same as the previous question, but $$\left \{ \vec{u},\vec{v} \right \}$$ is L.I.
    and $$\left \{\phi(\vec{u}), \phi(\vec{v})\right \}$$ is L.D.\
    What can one say about the range?

47. Note that range of a L.I function is always a subspace.

48. Note that the set N=$$\{\vec{v}: \phi(\vec{v})=0\}$$ is a subspace of $$R^2$$ where
    $$\phi:\mathbb{R}^2\rightarrow \mathbb{R}^2$$ is L.I . Take atleast 5
    different examples of L.I functions and see if this is true. The set
    $$N\subseteq Domain$$ is called the null space of $$\phi$$.

49. Construct a Linear Transformation
    $$\phi:\mathbb{R}^2\rightarrow \mathbb{R}^2$$, 
    $$\phi(0,1)=(3,4)$$ and $$\phi(1,0)=(1,2)$$. Construct an inverse of
    linear transformation and observe it carefully. Is it a L.T function
    too?

50. Do you realize the importance of inverting a matrix?

51. L.T stands for Linear Transformation .It is aka a matrix.

52. Define a L.T. $$\phi:\mathbb{R}^2\rightarrow \mathbb{R}^2$$ such that
    $$\phi(0,1)=(2,3)$$ and $$\phi(1,0)=(7,4)$$. This function $$\phi$$ is same
    as the matrix $$\begin{bmatrix}
    7 & 2 \\ 
    4 & 3
    \end{bmatrix}$$. 
	<br> $$\phi(x,y)$$ is same as $$\begin{bmatrix}
    7 & 2 \\ 
    4 & 3
    \end{bmatrix}$$ $$\begin{bmatrix}
    x\\y 
    \end{bmatrix}$$, Verify and make your share of observations. <br>
	What is
    $$\phi^{-1}$$ ? Is this the traditional matrix inverse?
    <br>Think !

53. Consider a L.T. $$\phi$$ such that : $$\phi(1,2)=(3,5)$$ and
    $$\phi(3,1)=(8,2)$$. What is the matrix equivalent of $$\phi$$ ?

54. Solve the following :
	- $$\begin{array} 3x-2y=15 \\ x+4y=19 \end{array}$$
		

    - Isn't this the same as $$\begin{bmatrix}
    1 & -2 \\ 
    1 & 4
    \end{bmatrix}$$ $$\begin{bmatrix}
    x\\y 
    \end{bmatrix}$$ = $$\begin{bmatrix}
    15\\19
    \end{bmatrix}$$

    - You are trying to find if there is an element in the domain
    which maps to (15,19) .

    - what exactly is happening here ? (Say all that you can)  

	<br>

55. Given $$\overrightarrow{V}_{1}$$ , $$\overrightarrow{V}_{2}$$ & $$\overrightarrow{V}_{3}$$ are L.I. , S.T.

    - $$\left \{ \overrightarrow{V}_{2} - \overrightarrow{V}_{3} , \overrightarrow{V}_{1} - \overrightarrow{V}_{3} , \overrightarrow{V}_{1} - \overrightarrow{V}_{2} \right \}$$
    are L.D.

    - $$\left \{ \overrightarrow{V}_{1} + \overrightarrow{V}_{2} , \overrightarrow{V}_{1} + \overrightarrow{V}_{3} , \overrightarrow{V}_{2} + \overrightarrow{V}_{3} \right \}$$
    are L.I.

56. Given vectors $$\left \{ \overrightarrow{V}_{1} , \overrightarrow{V}_{2} , \overrightarrow{V}_{3} , \overrightarrow{V}_{4} \right \}$$
    their sum is 0 = $$\overrightarrow{V}_{1}$$ + $$\overrightarrow{V}_{2}$$ + $$\overrightarrow{V}_{3}$$ + $$\overrightarrow{V}_{4}$$ . Is this set
    L.I or L.D. ?

57. Show that the following are equivalent:

    - The vectors $$\{\vec{v}_1,\vec{v}_2,\dots, \vec{v}_n\}$$ are linearly independent.<br>

    - $$\forall \alpha_1, \alpha_2, \dots, \alpha_n \in \mathbb{R}\  \left( \sum_{i=1}^{n} \alpha_i \vec{v}_i = 0 \implies \alpha_j = 0\ \forall 1 \leq j \leq n\right)$$.<br>

58. In the following six matrices find out the following:

    1.  Rank of the matrix

    2.  Dimension of the range

        1.  $$\left[ \begin{array}{cc}
            1 & 2\\ 2 & 4
            \end{array}\right]$$

        2.  $$\left[ \begin{array}{cc}
            1 & 2\\ 3 & 4
            \end{array}\right]$$

        3.  $$\left[ \begin{array}{cc}
            7 & -7\\ 2 & -2
            \end{array}\right]$$

        4.  $$\left[ \begin{array}{cc}
            0 & 1\\ 1 & 0
            \end{array}\right]$$

        5.  $$\left[ \begin{array}{cc}
            1 & 1\\ 3 & 3
            \end{array}\right]$$

        6.  $$\left[ \begin{array}{ccc}
            1 & 2 & 3\\ 4 & 5  &  6 \\ 7 & 8 & 9
            \end{array}\right]$$

    What is happening here? Describe in detail.

59. The dimension of the range of the matrix $$M$$ and $$M^{T}$$ is always
    the same. Why?

60. Take three linearly independent vectors in $$\mathbb{R}^3$$. Show that
    they form a basis of $$\mathbb{R}^3$$.

61. Consider the matrix $$\left[ \begin{array}{ccc}
    1 & 4 & 7\\ 2 & 5  &  8 \\ 3 & 6 & 9
    \end{array}\right]$$. The dimension of the range is 2. The range of
    this linear transformation is obviously a linear combination of
    three vectors. Do you see which are those three vectors?

62. Consider any $$2 \times 2$$ matrix. Do you observe that the : 

    Dimension of the Null space & the Dimension of the range are in someway related?

63. What about a $$3 \times 3$$ matrix? 

64. Can you generalise this to an $$n\times n$$ matrix?

65. When is a L.T. function one-one and when is it onto?

66. A $$2\times 2$$ matrix A can be seen as two vectors placed as columns. For
    example $$(1,2)$$ and $$(3,4)$$ when placed as columns give rise to the
    matrix $$\begin{bmatrix}
    1 & 3 \\
    2 & 4 
    \end{bmatrix}$$.

    Note that $$\begin{bmatrix}
    1 & 3 \\
    2 & 4 
    \end{bmatrix}$$ $$\begin{bmatrix}
    \alpha \\
    \beta
    \end{bmatrix}$$ $$\in$$
    $${\{ \alpha(1,2)+\beta(3,4) : \alpha, \beta \in \mathbb{R} \} }$$.

    Note that matrix, $$\begin{bmatrix}
    a & b \\
    c & d 
    \end{bmatrix}$$ $$\begin{bmatrix}
    x \\
    y
    \end{bmatrix}$$ simply is $$x(a,c)+y(b,d)$$.

    Note that a matrix takes a vector $$(x,y)$$ to a linear combination of
    the column vectors.

    It is now clear that the range of the matrix, say$$\begin{bmatrix}
    1 & 1 & 4 \\
    0 & 2 & 4 \\
    1 & 3 & 4 
    \end{bmatrix}$$ is nothing but the linear combination of the vectors
    $$(1,0,1), (1,2,3), (4,4,4)$$.

67. Consider a $$10\times 10$$ matrix $$A$$, defined as following:

    $$A[i,j] = 0$$ if $$i+j\cong 0(mod2)$$

    $$A[i,j] = 1$$ if $$i+j\cong 1(mod2)$$

    What is the dimension of the range?

68. Consider the sub-space $$S:(y=13x)$$ of $$\mathbb{R}^2$$

    - Give an example of a $$\phi$$ such that $$S$$ is its null space.

    - Give an example of a $$\phi$$ such that $$S$$ is the the
        range of $$\phi$$.

69. Let $$A =$$ 
	$$\begin{bmatrix}
    1 & 3 \\
    2 & 4 
    \end{bmatrix}$$

    - Show that the null space of $$A \subset$$ Null space of $$A^2$$

    - Is this true for any $$2\times 2$$ matrix.

    - Is this true for any $$3\times3$$ matrix.

    - Is this true for any $$n\times n$$ matrix.

70. Define column space. S.T. Column space of $$A^2 \subset$$ Column space
    of $$A$$.

71. Solve the following simultaneous equation:
	<br>
	- $$
	\begin{array}  _x + 4y + 7z =9\\
	2x + 5y + 8z = 9\\
	3x +6y + 9z = 9
	\end{array}
	$$

    - What is the null space of $$\begin{bmatrix}
        1 & 4 & 7 \\
        2 & 5 & 8 \\
        3 & 6 & 9 
        \end{bmatrix}$$ 
	- The above two questions are strongly related and
        make a theory. What is your obseration?

72. What does one mean by the linear combination of vectors and what is a
    linear span?

73. Show that, if a matrix $$A$$ has linearly independent column vectors,
    then the columns of the matrix $$A^2$$ are also linearly independent.

74. $$A\vec{x} = A\vec{y} \iff \vec{x}=\vec{y}$$ . Is this true? If False, when is the statement
    False and what leads to the falsity of the statement?

75. Let $$M$$ be a $$3\times 3$$ matrix, such that, the dim(Range) =3. Show 
	that, $$M^2 = M \iff M$$ is an identity matrix.

76. Consider a $$10 \times 10$$ matrix with all its entries to be $$1$$.
    What is the dimension of its range?

# 2.6 - Matricies

3. Matrix opperations:
- The scalar product of $c\in\mathbb{R}$ and $A=[a_{ij}]_{m\times n}$ is $cA=[ca_ij]_{m\times n}$
- The sum of 
- the Product of $A=[a_ij]_{m\times k}$ and $B=[b_ij]_{k\times n}$ is $AB=[c_ij]_{m\times n}$
whos enteries consist of the linear combinations of the rows A with the columns of B. for $1\leq i\leq m$ and $1\leq i\leq n$
$c_ij=a_{i1}b_{1j}+a_{i2}b_{2j}+a_{i3}b_{3j}+...+a_{ik}b_{kj}$

4. Let $A=\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$ and $B=\begin{bmatrix} 5 & -1 \\ -2 & 6 \end{bmatrix}$
a) $2A=\begin{bmatrix} 2 & 4 \\ 6 & 8 \end{bmatrix}$
b) $A+3B=\begin{bmatrix} 16 & -1 \\ -3 & 22 \end{bmatrix}$
c) $AB=\begin{bmatrix} 1 & 11 \\ 16 & 21 \end{bmatrix}$
d) $BA=\begin{bmatrix} 2 & 6 \\ 16 & 20 \end{bmatrix}$

## 2.6.3 Transpses and powers of matricies 

5. The idenity amtrix of order n, denoted $I_n$ is the $n\times n$ matrix 
$I_n=\begin{bmatrix} 1 & 0 & \cdots & 0 \\ 0 & 1 & \cdots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \cdots & 1 \end{bmatrix}$

6. Let A be a square matrix and $n\in\mathbb{N}$. the n-th iteratie power of $A$, denoted $A^n$ is defined as $A^0=I$ and, for $n\in\mathbb{Z}^+$
$A^n=A A A ... A$, n times

7. Given a matrix A, if there exists a matrix B such that $AB=I$ and $BA=I$, then $A$ is invertible and $B$ is called the inverse of $A$

8. Show that $A=\begin{bmatrix} 7 & 3 \\ 2 & 1 \end{bmatrix}$ and $B=\begin{bmatrix} 1 & -3 \\ -2 & 7 \end{bmatrix}$

$ AB=\begin{bmatrix}7 & 3 \\ 2 & 1\end{bmatrix}\begin{bmatrix}1 & -3 \\ -2 & 7\end{bmatrix}=\begin{bmatrix}1 & 0 \\ 0 & 1\end{bmatrix}$

9. The transpose of $A=[a_ij]_{m\times n}$ denoted $A^t$, is $A^t=[a_ji]_{n\times m}$ 

(flip along the diagonal)

- A is symetric of $A=A^t$
- A is skew-symmetric if $A=-A^t$

10. Determine the transposes of 
$A=\begin{bmatrix} 1 & 0 & 2 \\ 3 & -1 & 4 \end{bmatrix}$
$A^t=\begin{bmatrix} 1 & 3 \\ 0 & -1 \\ 2 & 4 \end{bmatrix}$

$ B=\begin{bmatrix} 2& 5 & 0 \\ 5 & -4 & 3 \\ 0 & 3 & 0 \end{bmatrix}$
$ B^t=\begin{bmatrix} 2& 5 & 0 \\ 5 & -4 & 3 \\ 0 & 3 & 0 \end{bmatrix}$

$C=\begin{bmatrix} 0 & 5 & 1 \\ -5 & 0 & -3 \\ -1 & 4 & 0 \end{bmatrix}$
$C^t=-C$

11. Let $A=\begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}$ and $B=\begin{bmatrix} 5 & -1 \\ -2 & 6 \end{bmatrix}$
evaluate a)$(AB)^t$ b) $B^tA^t$

a)
$(AB)^t=\begin{bmatrix} 1 & 7 \\ 11 & 21 \end{bmatrix}$
b)
$A^t = \begin{bmatrix} 1 & 3 \\ 2 & 4 \end{bmatrix},\ B^t=\begin{bmatrix} 5 & -2 \\ -1 & 6\end{bmatrix}$

$ A^tB^t=\begin{bmatrix} 1 & 7 \\ 11 & 21\end{bmatrix}$

12. A matrix where all of its entries are either 0 or 1 is called a zero-one matrix (0,1) matrix

13. Bitwise stuff on matricies works ($\land,\ \lor$)


# Linear Algebra

## 1. Introduction to Matrices

- **D1** column vectors

  $\R^n=$ set of column vectors of height $n$ with **entries** $a_i\in\R$

- **D2** zero vector

  $\mathbf{0}_n=$ column vector of height $n$ with all entries $a_i=0$

- **D3** standard basis vectors

  $\mathbf{e}_k=$ column vector of height $n$ with $a_k=1$ and all other entries $a_i=0,i\neq k$

- **R1** 

  $\forall \mathbf{v},\mathbf{e}_k\in\R^n,\lambda\in\R,$

  - $\mathbf{v}+\mathbf{0}_n=\mathbf{0}_n+\mathbf{v}=\mathbf{v}$
  - $0\mathbf{v}=\lambda\mathbf{0}_n=\mathbf{0}_n$
  - $\mathbf{v}\cdot\mathbf{0}_n=0$
  - $\mathbf{v}\cdot\mathbf{e}_k=v_k$ ($k$th entry of $\mathbf{v}$)

- **D5** linear combination

  $\forall \mathbf{v}_1\ldots \mathbf{v}_k\in\R^n,c_1\ldots c_k\in\R,$

  $c_1\mathbf{v}_1+c_2\mathbf{v}_2+\ldots+c_k\mathbf{v}_k$ **(linear combination)**

- **D6** span

  $\forall \mathbf{v}_1\ldots \mathbf{v}_k\in\R^n,$

  - $span\{\mathbf{v}_1\ldots \mathbf{v}_k\}=$ the set of all linear combinations of $\mathbf{v}_1\ldots \mathbf{v}_k$

  - $\forall \mathbf{v}\in\R^n,\mathbf{v}\in span\{\mathbf{e}_1\ldots\mathbf{e}_n\}$

- **D7** length/norm

  $\forall\mathbf{v}\in\R^n,||\mathbf{v}||=\sqrt{\mathbf{v}\cdot\mathbf{v}}$

  - $||\mathbf{0}_n||=0$
  - $\mathbf{v}_n\neq\mathbf{0}_n\implies||\mathbf{v}||>0$

- **D8** unit vector

  $\mathbf{v}\in\R^n,||\mathbf{v}||=1$ **(unit vector)**

- **E3**
  - $\forall\mathbf{0}_n\neq\mathbf{v}\in\R^n,\mathbf{u}:=\frac{\mathbf{v}}{||\mathbf{v}||}$ is a unit vector **(normalizing)**
  - $\mathbf{e}_k$ are unit vectors

- **D9** distance

  $\forall\mathbf{u},\mathbf{v}\in\R^n,dist(\mathbf{u},\mathbf{v}):=||\mathbf{u}-\mathbf{v}||$

- **D10** matrix

  - an $n\times m$ matrix has $n$ rows and $m$ columns
  - column vectors of height $n$ are $n\times 1$ matrices
  - row vectors of length $n$ Are $1\times n$ matrices

- **D11** matrix entries

  - The $(i,j)$ entry of a matrix is the entry in row $i$ and column $j$
  - $M=(a_{ij})$ is a matrix whose $(i,j)$ entry is $a_{ij}$

- **D12** zero matrix

  $\mathbf{0}_{n\times m}=$ matrix with all entries $a_{ij}=0$

- **D14** transpose
  - $\forall A=(a_{ij}),A^T=(a_{ji})$
  - Transpose = reflexion in the **leading diagonal** (the $(1,1),(2,2),\ldots$ entries)
  - $(A^T)^T=A$

- **D16** identity matrix

  - $I_n:=(a_{ij})\in\R^{n\times n}:\forall 1\leq i,j\leq n,a_{ij}=\begin{cases}0,i\neq j\\1,i=j\end{cases}$

  - Identity matrix = square matrix with entries on the leading diagonal 1 and the rest 0

- **D17** matrix-vector multiplication

  $\forall A=(a_{ij})\in\R^{n\times m},\mathbf{v}\in\R^m,$

  $A\mathbf{v}\in\R^n$ with $k$th entry $=\sum^m_{j=1}a_{kj}v_j=\mathbf{v}\cdot(k$th row of $A)^T$

- **L1** $k$th column of a matrix

  $\forall A\in\R^{n\times m},\mathbf{e}_k\in\R^m,$

  $A\mathbf{e}_k\in\R^n=$ the $k$th column of $A$

- **E8**
  
  - $i$th row of $I_n=(\mathbf{e}_i)^T$
  - $\forall\mathbf{v}\in\R^n,I_n\mathbf{v}=\mathbf{v}$
  
- **E9**

  $\forall\mathbf{u}_1\ldots\mathbf{u}_m\in\R^n,\mathbf{x}\in\R^m,$ let $A:=(\mathbf{u}_1\ldots\mathbf{u}_k)\in\R^{n\times m},$

  $A\mathbf{x}=x_1u_1+\ldots+x_mu_m$ is the linear combination of $\mathbf{u}_1\ldots\mathbf{u}_m$

  

## 2. Systems of Linear Equations

- **D20** solutions to linear system of equations

  A **consistent** system has solutions where **inconsistent** ones do not.

- **L2/D21** coefficient and augmented matrix

  - $\forall A=(a_{ij})\in\R^{n\times m}$ **(coefficient matrix)** $,\mathbf{b}\in\R^n,\mathbf{v}\in\R^m$

    $(v_1\ldots v_m)$ is a solution to the system $\iff A\mathbf{v}=\mathbf{b}$

  - $(A|\mathbf{b})=$ adding $\mathbf{b}$ as an extra column to $A$ **(augmented matrix)**

- ==**D22** row operation==

  - $r_i(\lambda):$ multiply the $i$th row by $0\neq\lambda\in\R$
  - $r_{ij}:$ swap row $i$ with row $j$
  - $r_{ij}(\lambda):$ add $\lambda$ times row $i$ to row $j$

- **P1** operations do not affect solutions

  Let $(A|\mathbf{b})\xrightarrow{r}(A'|\mathbf{b}'),A\mathbf{v}=\mathbf{b}\iff A'\mathbf{v}=\mathbf{b}'$ 

- **D23** leading entry

  The left-most non-zero entry in a non-zero row

- ==**D24/25** echelon form/**row reduced echelon (RRE) form**==
  - The leading entry in each non-zero row equals 1
  - The leading 1 in each non-zero row is to the right of the leading 1 in any rows above
  - All zero rows are below all non-zero rows
  - **The leading 1 in each non-zero row is the only non-zero entry in its column**

- **E14** cases of RRE form

  Consider $(A|\mathbf{b})$ representing a system of linear equations in matrix form,

  - $A=I_n:\mathbf{b}$ is a unique solution
  - $A=\begin{pmatrix}I_n\\\mathbf{0}_{k\times n}\end{pmatrix}$
    - $\forall n<i\leq n+k,b_i=0:\mathbf{b}$ is a unique solution
    - Otherwise, the system is inconsistent
  - The $i$th column does not contain a leading 1
    - The variable $x_i$ can be set to any values **(free variable**, as opposed to **basic variable)**
    - The system has $\infin$ solutions **(underdetermined)**

- **D26** pivots
  - Pivot position = a leading entry in a matrix in RRE form
  - Pivot column = a column containing a pivot position

- **P2** put any matrix $A=(a_{ij})$ into RRE form

  - **Forward phase**: put into echelon form

    Starting from the first row, for each non-zero column $k,$

    1. Find a row $j$ such that $a_{jk}\neq0,$ multiply it by $a^{-1}_{jk}$ (to get a leading 1) and swap with the current row;
    2. Subtract $a_{j'k}$ times the current row from each succeeding row $j'$ to create 0s;
    3. Move on to the next row.

  - **Backward phase**: put into RRE form

    Starting from the bottom row,

    1. If the leading 1 is at the $k$th row, subtract $a_{jk}$ times the current row from each preceding row $j$ to clear the column;
    2. Move on to the previous row.

  - The RRE form of a matrix is unique

- **P3** number of solutions

  A system of linear equations has either $0,1,\infin$ solutions

  


## 3. Matrix Multiplication

- **D27** matrix multiplication

  $\forall A=(a_{ij})\in\R^{n\times m},B=(b_{ij})\in\R^{m\times l},$

  $AB=(p_{ij})\in\R^{n\times l}:p_{ij}=\sum^m_{k=1}a_{ik}b_{kj}$

- **R3** remarks for matrix multiplication

  Let rows of $A$ be $\mathbf{r}_1\ldots\mathbf{r}_n\in\R^m$ and columns of $B$ be $\mathbf{c}_1\ldots\mathbf{c}_l\in\R^m,$

  - The $(i,j)$ entry of $AB=\mathbf{r}^T_i\cdot\mathbf{c}_j$
  - The $j$th column of $AB=A\mathbf{c}_j$
  - $AB$ is defined $\iff$ number of columns of $A=$ number of rows of $B$

- **E17/L3** matrix multiplication as functions

  - $\forall A\in\R^{n\times m},\exist T_A:\R^m\rightarrow\R^n,\mathbf{v}\mapsto A\mathbf{v}$

  - $T_B:\R^l\rightarrow\R^m,T_A\circ T_B=T_{AB}:\R^l\rightarrow\R^n$

  - $\forall\mathbf{v}\in\R^l,A(B\mathbf{v})=(AB)\mathbf{v}$

- ==**P4** properties of matrix multiplication==

  $\forall A,A'\in\R^{m\times n},B,B'\in\R^{n\times p},C\in\R^{p\times q},\lambda\in\R$

  - $A(BC)=(AB)C$ **(associativity)**

  - $A(B+B')=AB+AB'$ **(left distributivity)**

    $(A+A')B=AB+A'B$ **(right distributivity)**

  - $(\lambda A)B=\lambda(AB)=A(\lambda B)$

  - Not commutative

  - $AB=0\centernot\implies A=\mathbf{0}_{m\times n}\or B=\mathbf{0}_{n\times p}$

- **L4** behaviour of zero and identity matrices

  $\forall A\in\R^{n\times m},$

  - $\forall k,\mathbf{0}_{k\times n}A=\mathbf{0}_{k\times m},A\mathbf{0}_{m\times k}=\mathbf{0}_{n\times k}$
  - $I_nA=AI_m=A$

- **D28** diagonal matrix

  $D=(d_{ij})\in\R^{n\times n}:\forall i\neq j,d_{ij}=0$ (all entries 0 other than leading diagonal)

  - $\forall n,I_n$ and $\mathbf{0}_{n\times n}$ are diagonal

  - Let $D:=diag(d_1,\ldots,d_n),D':=diag(d'_1,\ldots,d'_n),$

    $DD'=diag(d_1d'_1,\ldots,d_nd'_n)$

- **D29** triangular matrix

  $\forall A=(a_{ij}),$

  - $\forall i>j,a_{ij}=0$ **(upper triangular)**
  - $\forall i\geq j,a_{ij}=0$ **(strictly upper triangular)**
  - $\forall i<j,a_{ij}=0$ **(lower triangular)**
  - $\forall i\leq j,a_{ij}=0$ **(strictly lower triangular)**

- **E22** special triangular matrices

  -  $A$ is both upper and lower triangular $\iff A$ is diagonal
  - $A$ is both strictly upper and strictly lower triangular $\iff A=\mathbf{0}_{n\times n}$

- **D30** inverse matrix

  $\forall A\in\R^{n\times n},$

  - $\exist A^{-1}\in\R^{n\times n}:AA^{-1}=A^{-1}A=I_n$ ($A$ **invertible**)
  - $\not\exist A^{-1}$ ($A$ **singular**)

- **L5** uniqueness of inverse matrix

  - $A$ **invertible** $\implies\exist!A^{-1}$
  - $A$ **invertible** $\land(\exist B\in\R^{n\times n}:AB=I_n\lor BA=I_n)\implies B=A^{-1}$

- **L6** inverse of matrix product

  $(AB)^{-1}=B^{-1}A^{-1}$

- **L7/C1/C2** cases of singularities

  $\forall A=(a_{ij})\in\R^{n\times n},$

  - $\exist\mathbf{0}_n\neq\mathbf{v}\in\R^{n\times n}:A\mathbf{v}=\mathbf{0}_n\implies A$ **non-invertible**
  - $\exist\mathbf{0}_{n\times n}\neq B\in\R^{n\times n}:AB=\mathbf{0}_{n\times n}\lor BA=\mathbf{0}_{n\times n}\implies A$ **non-invertible**
  - $\exist k:(\forall i,a_{ik}=0)\lor(\forall j,a_{kj}=0)\implies A$ **non-invertible**

- **E23** determinant

  $\forall A=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\R^{2\times 2}$

  - $A^{-1}=\frac{1}{ad-bc}\begin{pmatrix}d&-b\\-c&a\end{pmatrix}$
  - $A$ **invertible** $\iff ad-bc\neq0$ **(determinant)**

- **D31/R4** elementary matrix

  - $I_n\xrightarrow{r}R$ (differs by one row operation from identity matrix)

  - $R$ **invertible**:
    - $R_i(\lambda)^{-1}=diag(1,\ldots,1,\lambda^{-1},1,\ldots,1)=R_i(\lambda^{-1})$
    - $R_{ij}^{-1}=R_{ij}$
    - $R_{ij}(\lambda)^{-1}=R_{ij}(-\lambda)$

- **L8/L9/P5** matrix invertability after row operations

  $\forall A\in\R^{n\times n},$

  - $A\xrightarrow{r}A',A$ **invertible** $\iff A'$ **invertible**
  - $A':=A$ in RRE form, $A'$ **invertible** $\iff A'$ has no zero rows
  - $A':=A$ in RRE form, $A$ **invertible** $\iff A'=I_n$
  - $A$ **invertible** $\iff\not\exist\mathbf{0}_n\neq\mathbf{v}\in\R^n:A\mathbf{v}=\mathbf{0}_n$

- **E24** compute inverse matrix

  If $A$ **invertible**, $(A|I_n)\xrightarrow{RRE}(I_n|A^{-1})$

  

## 4. Vector Spaces

- **D4.1** vector space

  - a set $V, v\in V$ are referred as "vectors"
  - binary operation $+:V\times V\rightarrow V$ **(addition)**
  - function $\R\times V\rightarrow V$ **(scalar multiplication)**

  With the following axioms hold $\forall \mathbf{u},\mathbf{v},\mathbf{w}\in V,\lambda_1,\lambda_2\in\R$:

  - **(A1)** $(\mathbf{u}+\mathbf{v})+\mathbf{w}=\mathbf{u}+(\mathbf{v}+\mathbf{w})$ 
  - **(A2)** $\mathbf{u}+\mathbf{v}=\mathbf{v}+\mathbf{u}$
  - **(A3)** $\exist\mathbf{0}_V\in V:\mathbf{u}+\mathbf{0}_V=\mathbf{u}$
  - **(A4)** $\exist-\mathbf{u}\in V:\mathbf{u}+(-\mathbf{u})=\mathbf{0}_V$
  - **(M1)** $\lambda_1(\lambda_2\mathbf{u})=(\lambda_1\lambda_2)\mathbf{u}$
  - **(M2)** $(\lambda_1+\lambda_2)\mathbf{u}=\lambda_1\mathbf{u}+\lambda_2\mathbf{u}$
  - **(M3)** $\lambda_1(\mathbf{u}+\mathbf{v})=\lambda_1\mathbf{u}+\lambda_1\mathbf{v}$
  - **(M4)** $1\cdot\mathbf{u}=\mathbf{u}$

- **E4.1** some examples of vector spaces

  $\R,\R^n,\R[X]\sub\R^\R:=\{f:\R\rightarrow\R\},\R^{n\times m},\R^0=\{\mathbf{0}_V\}$

- **L4.1** more properties of vector spaces

  $\forall\mathbf{x}\in V$ a vector space,

  - $\forall n\in\N,n\mathbf{x}=\mathbf{x}+\mathbf{x}+\ldots+\mathbf{x}$ (n terms)
  - $0\mathbf{x}=\mathbf{0}_V$
  - $\mathbf{x}+(-1)\mathbf{x}=\mathbf{0}_V$ (**additive inverse**)

- **D4.2** subspace

  A subset $U\sub V:$

  - $\mathbf{0}_V\in U$ (not empty)
  - $\forall \mathbf{x},\mathbf{y}\in U,\mathbf{x}+\mathbf{y}\in U$
  - $\forall \mathbf{x}\in U,\forall\lambda\in\R,\lambda\mathbf{x}\in U$

- **E4.2** proper subspace

  $\forall V$ a vector space, $V$ and ${\mathbf{0}_V\sub V}$ **subspaces**, all other subspaces are **proper subspaces**

- **L4.2/E4.3** operations of subspaces

  $\forall V$ a vector space, $\forall U,W\in V$ **subspaces**,

  - $U\cap W$ **subspace**
  - $U\cup W$ **subspace** $\iff U\sube W\lor W\sube U$
  - $U+W:=\{\mathbf x+\mathbf y|\mathbf x\in U,\mathbf y\in W\}$ **subspace**

- **D4.3** linear combination

  $\forall\mathbf{v}_1\cdots\mathbf{v}_n\in S\sub V$ a vector space, $\lambda_1\ldots\lambda_n\in\R,$

  $\lambda_1\mathbf{v}_1+\lambda_2\mathbf{v}_2+\ldots+\lambda_n\mathbf{v}_n$ **(linear combination)**

- ==**D4.4** span==

  $\forall S\sub V$ a vector space,

  $span(S)=\begin{dcases}\mathbf{0}_V&S=\empty\\all\phantom{.}linear\phantom{.}combinations\phantom{.}of\phantom{.}\mathbf{v}_1\cdots\mathbf{v}_n\in S&otherwise\end{dcases}$

- **L4.3** subspace with linear combination

  $\empty\neq U\sub V$ **subspace** $\iff \forall\mathbf{x}\in span(U),\mathbf{x}\in U$

- **L4.4** span and subspace

  $\forall S\sub V$ a vector space, $span(S)$ **subspace**

- ==**D4.5/E4.5** spanning set==

  $\forall S\sub V$ a vector space,

  $span(S)=V\implies S$ **spanning set**

  - $\{\mathbf{e}_1\ldots\mathbf{e}_n\}\sub\R^n$ **spanning set**
  - $\{1\}\cup\{X^n|n\in\N\}\sub\R[X]$ **spanning set**
  - $S=V$ **spanning set**

- **L4.5** span in subspace

  $\forall S\sub V$ a vector space, $U\sub V$ **subspace**,

  $S\sub U\implies span(S)\sub U$

- **D4.6** finite-dimensional

  $\forall V$ a vector space,

  $\exist S$ **finite spanning set** $\implies V$ **finite dimensional**

- **E4.7** infinite dimensional

  $\R[X]$ (proof by contradiction)

- ==**D4.7** dimension==

  $\forall V$ **finite-dimensional** vector space,

  $\dim V=$ size of smallest **spanning set** of $V$

- ==**D4.8/E4.10** linear dependence==

  $\forall\mathcal{L}\sub V$ a vector space,

  $\exist\text{(distinct)}\mathbf{v}_1\ldots\mathbf{v}_n\in\mathcal{L},\lambda_1\ldots\lambda_n\in\R\backslash\{0\}:\sum^n_{i=1}\lambda_i\mathbf{v}_i=\mathbf{0}_V\implies\mathcal{L}\textbf{ linearly dependent}$
  
  - $\empty\sub V\textbf{ linearly independent}$
  - $\forall\mathcal{L'}\sub\mathcal{L},$
    - $\mathcal{L'}\textbf{ linearly dependent}\implies\mathcal{L}\textbf{ linearly dependent}$
    - $\mathcal{L}\textbf{ linearly independent}\implies\mathcal{L'}\textbf{ linearly independent}$
  - $\mathbf{0}_V\in\mathcal{L}\implies\mathcal{L}\textbf{ linearly dependent}$
  - $\exist\text{(distinct)}\mathbf{x},\mathbf{y}\in\mathcal{L},\lambda\in\R:\mathbf{x}=\lambda\mathbf{y}\implies\mathcal{L}\textbf{ linearly dependent}$

- ==**D4.9/E4.11** bases==

  A **basis** of a vector space is a **linearly independent spanning set**

  - $\{\mathbf{e}_1\ldots\mathbf{e}_n\}\sub\R^n$ (**standard basis**)
  - $\empty\sub\{0\}$ **basis**
  - $\{1,X,\ldots,X^d\}\sub\R[X]_{\leq d}$ **basis**
  - $\{1\}\cup\{X^n|n\in\N\}\sub\R[X]$ **basis**

- **P4.6/E4.12** basis characterisation

  $\forall\mathcal{B}=\{\mathbf{v}_1\ldots\mathbf{v}_n\}\sub V$ a vector space,

  $\mathcal B$ **basis** $\iff\forall\mathbf{x}\in V,\mathbf{x}$ equals a unique **linear combination** of $\mathcal{B}$

  - $\mathbf{x}=\sum^n_{i=1}\lambda_i\mathbf{v}_i,(\{\lambda_i\}\textbf{ coefficients}\text{ of }\mathbf{x}\text{ with respect to }\mathcal{B})$

    **bijection** $F_\mathcal{B}:\R^n\rightarrow V,\begin{pmatrix}\lambda_1\\\vdots\\\lambda_n\end{pmatrix}\mapsto\sum^n_{i=1}\lambda_i\mathbf{v}_i$ (isomorphism)

- **L4.7** smaller within linear dependent spanning set

  $\forall S\sub V$ **linearly dependent spanning set**, 

  $\exist\mathbf{x}\in S:S'=S\backslash\{\mathbf{x}\}$ **spanning set**

- **C4.8** 

  Any **finite spanning set** contains a **basis**

- **C4.9** 

  Any **finite-dimensional** vector space has a **basis**

- **P4.10** easy Steinitz exhange lemma

  $\forall S\sub V$ **spanning set**, $\forall\mathbf{0}_V\neq\mathbf{x}\in V,\exist\mathbf{y}\in S:S'=(S\backslash\{\mathbf{y}\})\cup\{\mathbf{x}\}$ **spanning set**

- **P4.11** full Steinitz exhange lemma

  $\forall S\sub V$ **spanning set**, $\mathcal{L}=\{\mathbf{x}_1\dots\mathbf{x}_n\}\sub V$ **linearly independent**, $\exist\mathcal{T}=\{\mathbf{y}_1\ldots\mathbf{y}_n\}\sub S:S'=(S\backslash\mathcal{T})\cup\mathcal{L}$ **spanning set**

- **C4.12**

  $\forall V$ **finite-dimensional** vector space, $\mathcal{L}\sub V$ **linearly independent**, $S\sub V$ **finite spanning set** $\implies\mathcal L$ **finite**: $\#\mathcal L\leq\# S$

- ==**T4.13/L4.16** size of basis is dimension of vector space==

  $\forall V$ **finite-dimensional** vector space, $\dim V=n,$

  - $\forall\mathcal B\sub V,\mathcal B$ **basis** $\implies\mathcal B$ **finite**: $\#\mathcal{B}=n$
  - $\forall\textbf{ linearly independent }\mathcal L\sub V,\#\mathcal L=n\implies\mathcal L$ **basis**

- **L4.14**

  $\forall\mathcal{L}\sub V$ **linearly independent**, $\mathbf{v}\in V$

  $\mathbf{v}\notin\mathcal L\implies\mathcal L\cup\{\mathbf{v}\}$ **linearly independent**

- **L4.15**

  $\forall V$ **infinite-dimensional** vector space,

  $\forall n\in\N,\exist\textbf{ linearly independent }\mathcal L\sub V:\mathcal \#\mathcal L=n$

- **L4.17**

  $\forall V$ **finite-dimensional** vector space,

  $\forall\textbf{ linearly independent }\mathcal L\sub V,\exist\textbf{ basis }\mathcal B:\mathcal{L}\sub\mathcal{B}$

  - An linearly independent subset can be **extending to a basis** by adding in more vectors

- **P4.18**

  $\forall V$ **finite-dimensional** vector space, $U\sub V$ **subspace**,

  - $U$ **finite-dimensional**
  - $\dim U\leq\dim V$
  - $\dim U=\dim V\implies U=V$



## 5. Linear Maps

- **D5.1** linear map

  $\forall U,V$ vector spaces, $f:U\rightarrow V$ **linear map** if

  - $\forall\mathbf x,\mathbf y\in U,f(\mathbf x+\mathbf y)=f(\mathbf x)+f(\mathbf y)$ **and**
  - $\forall \mathbf x\in U,\forall\lambda\in\R,f(\lambda\mathbf x)=\lambda f(\mathbf x)$

- **E5.1** examples of linear map

  - ==$\forall A\in\R^{n\times k},T_A:\R^k\rightarrow\R^n,\mathbf v\mapsto A\mathbf v$==
  - $\forall V$ vector space, $id_V:V\rightarrow V$
  - $\forall U,V$ vector spaces, **zero map**: $U\rightarrow V,\mathbf x\mapsto\mathbf 0_V$
  - $D:\R[X]\rightarrow\R[X],P\mapsto\frac{dP}{dX}\\$ 

- **L5.1** linear map and zero vectors

  $f:U\rightarrow V$ **linear** $\implies f(\mathbf 0_U)=\mathbf 0_V$

- **L5.2** composing linear maps

  $f:U\rightarrow V,g:V\rightarrow W$ **linear maps** $\rightarrow g\circ f:U\rightarrow W$ **linear**

- ==**D5.2/5.4/T5.14** image (rank) and kernel (nullity)==

  $\forall f:U\rightarrow V$ **linear**

  - $\text{Im} f=\{f(\mathbf u)|\mathbf u\in U\}\sub V\qquad\text{rank }f=\dim(\text{Im }f)$
  - $\ker f=\{\mathbf u\in U,f(\mathbf u)=\mathbf 0_V\}\sub U\qquad\text{null }f=\dim(\ker f)$
  - ==$\text{rank }f+\text{null }f=\dim U$==

- **L5.3** image/kernel are subspaces

  $\forall f:U\rightarrow V$ **linear**

  - $\text{Im} f\sub V$ **subspace**
  - $\ker f\sub U$ **subspace**

- **L5.4** injectivity with kernel

  $\forall f:U\rightarrow V$ **linear**,

  $f$ **injective** $\iff\ker f=\{\mathbf 0_U\}$

- **L5.5**

  $\forall f:U\rightarrow V$ **linear**, $\mathbf y\in V,$

  $\exist\mathbf x\in U:f(\mathbf x)=\mathbf y\implies f^{-1}(\mathbf y)=\{\mathbf x+\mathbf v|\mathbf v\in\ker f\}$

  (all other elements in the pre-image of $\mathbf y$ can be obtained by adding vectors in $\ker f$ to some $\mathbf x$ s.t. $f(\mathbf x)=\mathbf y$)

- **P5.6**

  $f:\R^k\rightarrow\R^n$ **linear** $\implies \exist A\in\R^{n\times k},f=T_A$

- **P5.7**

  $\forall f:U\rightarrow V,g:U\rightarrow V$ **linear maps**, $\mathcal B=\{\mathbf b_1\ldots\mathbf b_k\}\sub U$ **basis**, 

  $f(\mathbf b_i)=g(\mathbf b_i)\forall 1\leq i\leq k\implies f=g$

- **P5.8**

  $\forall U,V$ vector spaces, $\mathcal B=\{\mathbf b_1\ldots\mathbf b_k\}\sub U$ **basis**, $\forall\{\mathbf v_1\ldots\mathbf v_k\}\sub V,$

  $\exist!f:U\rightarrow V$ **linear**: $f(\mathbf b_i)=\mathbf v_i\forall 1\leq i\leq k$

  (a linear map can be defined unambiguously by specifying what it does to a basis, aka. **extending linearly**)

- **D5.3** isomorphism

  - $\forall f:U\to V$ **linear map**, 

    $f\textbf{ bijective}\iff f\textbf{ isomorphism}$

  - $\exist\textbf{ isomorphism }f:U\to V\implies U\cong V$ (U is **isomorphic** to V)

- **P5.9** isomorphic with dimensions

  $\forall V\text{ a vector space},$

  $\dim V=n\implies V\cong\R^n$

- **L5.10**

  $\forall f:U\to V\textbf{ linear map},\mathcal B=\{\mathbf b_1\ldots\mathbf b_k\}\sub U\textbf{ basis},\mathcal C=\{f(\mathbf b_1)\ldots f(\mathbf b_k)\}\sub V,$

  - $\mathcal C\textbf{ spanning set}\iff f\textbf{ surjective}$
  - $\mathcal C\textbf{ linearly independent}\iff f\textbf{ injective}$
  - $\mathcal C\textbf{ basis}\iff f\textbf{ isomorphism}$

- **C5.11**

  $U\cong V\implies\dim U=\dim V$

- **C5.12**

  $\forall f:U\to V\textbf{ linear map},\dim U=\dim V\implies$

  $f\textbf{ injective}\iff f\textbf{ surjective}\iff f\textbf{ isomorphism}$

- **C5.13**

  $\forall f:\R^n\to V\textbf{ isomorphism},$

  $\mathcal C=\{f(\mathbf e_1)\ldots f(\mathbf e_n)\}\sub V\textbf{ basis}$

- **D** representing linear map by matrix

  $\forall\textbf{linear map }f:U\to V,\forall\textbf{basis }\mathcal B=\{\mathbf b_1\ldots\mathbf b_k\}\sub U,\forall\textbf{basis }\mathcal C=\{\mathbf c_1\ldots \mathbf c_n\}\sub V,$

  $\exist\textbf{matrix }{}_\mathcal C[f]_\mathcal B: F_\mathcal C^{-1}\circ f\circ F_\mathcal B(\mathbf v)={}_\mathcal C[f]_\mathcal B\cdot\mathbf v$ (matrix representing $f$ with respect to $\mathcal B$ and $\mathcal C$)

  - Express each $f(\mathbf b_j)$ as a linear combination of $\sum_{i=0}^n a_{ij}\mathbf c_i\\$ for some scalars $a_{ij}\in\R,$ then ${}_\mathcal C[f]_\mathcal B=(a_{ij})$

- **E5.11**

  $\forall M\in\R^{n\times k},T_M:\R^k\to\R^n,\textbf{standard bases }\mathcal B\sub\R^k,\mathcal C\sub\R^n,$

  $\implies{}_\mathcal C[T_M]_\mathcal B=M$

- **D5.5** change-of-basis matrix

  $\forall V\text{ a vector space},\forall\textbf{basis }\mathcal{B,C}\sub V,$

  **change-of-basis** matrix from $\mathcal B$ to $\mathcal C$ is ${}_\mathcal C[id_V]_\mathcal B=:{}_\mathcal CP_\mathcal B$

- **L5.15**

  $\forall V\text{ a vector space},\forall\textbf{basis }\mathcal{B,C}\sub V,P:={}_\mathcal C[id_V]_\mathcal B,\forall\mathbf x\in V,$

  The coefficients of $\mathbf x$ wrt $\mathcal B$ is $\mathbf v\in\R^n$

  $\implies$ the coefficients of $\mathbf x$ wrt $\mathcal C$ is $P\mathbf v$

- **E5.12** inverse of change-of-basis matrix

  $\forall\textbf{basis }\mathcal{B,C}\sub V,$

  $({}_\mathcal CP_\mathcal B)^{-1}={}_\mathcal BP_\mathcal C$

- **P5.16** change-of-basis formula

  $\forall\textbf{linear map }f:U\to V,\forall\textbf{bases }\mathcal {B,B'}\sub U,\textbf{bases }\mathcal {C,C'}\sub V,$

  ${}_{\mathcal C'}[f]_{\mathcal B'}={}_{\mathcal C'}P_\mathcal C\,{}_\mathcal C[f]_\mathcal B\,{}_\mathcal BP_{\mathcal B'}\,{}$

  

## 6. Introduction to determinants

- **D1** minor

  $\forall A\in\R^{n\times n},A_{ij}$ (**minor**) is the sub matrix obtained by deleting row $i$ and column $j$ from $A$.

- **D2** determinant

  $\forall A\in\R^{n\times n},$

  $\det A=\sum_j(-1)^{i+j}a_{ij}\det A_{ij}\\$ (expansion along the $i$-th row)

  $=\sum_i(-1)^{i+j}a_{ij}\det A_{ij}\\$ (expansion along the $j$-th column)

- **D3** inversion and sign of permutation

  $\forall\sigma\in S_n,$ 

  - an **inversion** is a pair $(i,j)\in\N\times\N:i<j\land\sigma(i)\geq\sigma(j)$
  - $sgn(\sigma):=\begin{dcases}-1&\text{number of inversions in }\sigma\text{ is odd}\\1&otherwise\end{dcases}$

- **D4** determinant alternative

  $\forall A\in\R^{n\times n},$

  $\det A=\sum_{\sigma\in S_n}sgn(\sigma)a_{1\sigma(1)}a_{2\sigma(2)}\ldots a_{n\sigma(n)}$

- **E3**

  - $\det(I_n)=1$

  - $\det(diag(d_1,\ldots,d_n))=d_1d_2\ldots d_n$

  - $\forall A=(a_{ij}),$

    $\exist i\forall j(a_{ij}=0)\lor\exist j\forall i(a_{ij}=0)\implies\det A=0$

- **P1**
  - $A\xrightarrow{r_{ij}}B\implies\det B=-\det A$
  - $A\xrightarrow{r_{i}(\lambda)}B\implies\det B=\lambda\det A$
  - $A\xrightarrow{r_{ij}(\lambda)}B\implies\det B=\det A$

- **P2**

  $\forall A\in\R^{n\times n},$

  - $\det A=\det A^T$
  - $\det AB=\det A\det B$

- **P3** invertibility and determinant

  $\forall A\in\R^{n\times n},$

  $A\textbf{ invertible}\iff\det A\neq0$



## 7. Eigenvalues and eigenvectors

- ==**D5/R1** eigenvalue and eigenvector==

  $\forall A\in\R^{n\times n},\lambda\in\R,$

  $\exist\mathbf v\in\R^n:A\mathbf v=\lambda\mathbf v\implies\begin{dcases}\lambda\textbf{ eigenvalue }\text{of }A\\\mathbf v\textbf{ eigenvector }\text{of }A\text{ (for }\lambda)\end{dcases}$

  - $\mathbf v\text{ eigenvector of }A\text{ with eigenvalue }\lambda\iff(A-\lambda I_n)\mathbf v=0$

- **E4**
  
  - $\forall\mathbf v\in\R^n,\mathbf v\text{ eigenvector of }I_n\text{ with eigenvalue 1}$
  - $\forall\mathbf v\in\R^n,\mathbf v\text{ eigenvector of }\mathbf 0_{n\times n}\text{ with eigenvalue 1}$
  - $\forall k\leq n,\mathbf e_k\text{ eigenvector of }diag(d_1,\ldots,d_n)\text{ with eigenvalue }d_k$
  - $\forall\mu\neq0,\begin{pmatrix}\mu\\\pm\mu\end{pmatrix}\text{ eigenvector of }\begin{pmatrix}1&2\\2&1\end{pmatrix}$
  
- **P4**

  $\forall A\in\R^{n\times n},$

  $\lambda\text{ eigenvalue of }A\iff A-\lambda I_n\textbf{ non-invertible}$

- **D6** characteristic polynomial

  $\forall A\in\R^{n\times n},$

  $p_A(\lambda):=\det(A-\lambda I_n)$

- ==**D7/L1** similarity==

  $\forall A,B\in\R^{n\times n},$

  $\exist\textbf{invertible }P:A=P^{-1}BP\implies A\textbf{ similar to }B\iff B\textbf{ similar to }A$

- **P5**

  Similar matrices have the same eigenvalues

- ==**D8** diagonalisability==

  $\forall A\in\R^{n\times n},$

  $\exist D=diag(d_1,\ldots,d_n),A\text{ similar to }D\implies A\textbf{ diagonalisable}$

- **L2/R3**

  $\forall A\in\R^{n\times n},\mathbf v_1\ldots\mathbf v_n\text{ eigenvectors of }A\text{ with eigenvalues }\lambda_1\ldots\lambda_n,P:=(v_1|\ldots|v_n),$

  $P\textbf{ invertible}\implies A\textbf{ diagonalisable}\text{ to }P^{-1}AP=diag(\lambda_1,\dots,\lambda_n)$

- **D9** eigenspace

  $\forall A\in\R^{n\times n}$
  
  $E_\lambda:=\{\mathbf v\in\R^n|A\mathbf v=\lambda\mathbf v\}$

- **P2.1/R4**

  Any eigenspace $E_\lambda$ of a matrix $A\in\R^{n\times n}$ is a subspace of $\R^n$

  - $E_\lambda=\ker(T_{A-\lambda I_n})=span\{\textbf v_1\ldots\textbf v_k\}$ where $\textbf v_1\ldots\textbf v_k$ are eigenvectors to the eigenvalue $\lambda$

- ==**D10/P2.2** orthogonal/orthonormal set==

  $\forall S=\{\textbf v_1\ldots\textbf v_n\}\in\R^n,$

  - $(\forall i\neq j,\textbf v_i\cdot\textbf v_j=0)\implies S\textbf{ orthogonal set}$
    - $\implies S\textbf{ linearly independent}$
  - $(S\textbf{ orthogonal}\land\forall\textbf v\in S,\textbf v\textbf{ unit})\implies S\textbf{ orthonormal}$ 
    - $\{\textbf{v}_1\ldots\textbf v_n\}\textbf{ orthogonal}\implies\{\frac{\mathbf v_1}{||\mathbf v_1||}\ldots\frac{\mathbf v_n}{||\mathbf v_n||}\}\textbf{ orthonormal}\\$

- **D11** orthogonal projection

  $\forall S=\{\mathbf v_1\ldots\mathbf v_k\}\in\R^n,U=span(S),y\in\R^n,$

  $proj_Uy:=\sum^k_{i=1}\frac{y\cdot\textbf v_i}{||\mathbf v_i||^2}\mathbf v_i\\$ (**orthogonal projection** of $y$ onto $U$)

- ==**T2.3** Gram-Schmidt Process==

  $\forall S=\{\mathbf v_1\ldots\mathbf v_k\}\in\R^n\textbf{ linearly independent},i\leq k:$

  - $\mathbf w_1:=\mathbf v_1$

  - $\mathbf w_2:=\mathbf v_2-proj_{span\{\mathbf w_1\}}\mathbf v_2=\mathbf v_2-\frac{\mathbf v_2\cdot\textbf w_1}{||\mathbf w_1||^2}\mathbf w_1\\$

  - $\mathbf w_3:=\mathbf v_3-proj_{span\{\mathbf w_1,\mathbf w_2\}}\mathbf v_3=\mathbf v_3-(\frac{\mathbf v_3\cdot\textbf w_1}{||\mathbf w_1||^2}\mathbf w_1+\frac{\mathbf v_3\cdot\textbf w_2}{||\mathbf w_2||^2}\mathbf w_2)\\$

    $\vdots$

  - $\mathbf w_k=\mathbf v_k-proj_{span\{\mathbf w_1\ldots\mathbf w_{k-1}\}}\mathbf v_k=\mathbf v_k-\sum^{k-1}_{i=1}\frac{\mathbf v_k\cdot\textbf w_i}{||\mathbf w_i||^2}\mathbf w_i\\$

  1. $\{\mathbf w_1\ldots\mathbf w_k\}\textbf{ orthogonal}$
  2. $\{\mathbf u_1\ldots\mathbf u_k|\mathbf u_i=\frac{\mathbf w_i}{||\mathbf w_i||}\}\textbf{ orthonormal}\\$
  3. $Span\{\mathbf w_1\ldots\mathbf w_k\}=Span\{\mathbf u_1\ldots\mathbf u_k\}=Span\{\mathbf v_1\ldots\mathbf v_k\}$

- **D12** orthogonal/orthonormal matrix
  - A matrix is **orthogonal** if its columns are an orthogonal set
    - An orthogonal matrix have **linearly independent** columns, and therefore always **invertible**
  - It is **orthonormal** if it is orthogonal and the columns are unit vectors

- **P2.4**

  $\forall A\in\R^{n\times n},$

  $A\textbf{ orthogonal}\iff AA^T=I_n$

- **D13** symmetric matrix

  $\forall A\in\R^{n\times n},$

  $A=A^T\implies A\textbf{ symmetric}$

- **T2.5** Fundamental Theorem of Algebra

  $\forall\text{non-constant } p\in\C[X],\exist x_0\in\C:p(x_0)=0$

- **P2.6**

  $\forall A\in\R^{n\times n}\textbf{ symmetric},$

  - $A$ has at least one eigenvalue $\in\R$
  - All $A$'s eigenvalues $\in\R$

- **L3**

  $\forall A\in\R^{n\times n}\textbf{ symmetric},\lambda_1\neq\lambda_2\textbf{ eigenvalues}\text{ corresponding }\mathbf v_1,\mathbf v_2,$

  $\implies \mathbf v_1,\mathbf v_2\textbf{ orthogonal}$

- **T2.7/R5/T2.8** spectral theorem

  $\forall A\in\R^{n\times n}\textbf{ symmetric},$

  $\iff A\textbf{ diagonalisable}\text{ with }\exist D=diag(d_1,\ldots,d_n),P\textbf{ invertible}:$

  $A=PDP^{-1}\land\text{matrix }P\text{ of eigenvectors}\textbf{ orthogonal}$

  $\iff A\textbf{ orthogonally diagonalisable}$



# Group Theory $\newcommand{\group}{\forall(G,\star)}$

## 1. Basic definitions and examples

- **D1** binary operation

  $\forall\text{set }G,$ a **binary operation** on $G$ is a function

  $\star:G\times G\to G$

- **R1** Carley table

  $\forall G=\{g_1,\ldots,g_n\},$ a binary operation on $G$ can be described by a multiplication (**Carley**) table:

  $\boxed{\begin{matrix}\star&g_1&g_2&\cdots&g_n\\g_1&g_1\star g_1&g_1\star g_2&\cdots&g_1\star g_n\\\vdots&&&&\vdots\\g_n&g_n\star g_1&g_n\star g_2&\cdots&g_n\star g_n\end{matrix}}$

  - The number of different binary operations on $G$ is $n^{n^2}$

- **D2** associativity

  $\forall g,h,k\in G,$

  $g\star(h\star k)=(g\star h)\star k\implies\star\textbf{ associative}$

- **D3** commutativity

  $\forall g,h\in G,$

  $g\star h=h\star g\implies\star\textbf{ commutative}$

- **D4** left/right identity element

  $\forall e\in G,$

  - $(\forall g\in G,e\star g=g)\implies e\textbf{ left identity element}$

  - $(\forall g\in G,g\star e=g)\implies e\textbf{ right identity element}$

- **P1** two sided identity element

  $\forall e_1\textbf{ left identity},e_2\textbf{ right identity}\in G,$

  $\implies e_1=e_2=:e$ (**two sided identity**)

- **P2** uniqueness of identity

  $\forall G,\exist e\textbf{ identity}\implies\exist! e\textbf{ identity}$

- **D5** left/right inverse

  $\forall e\textbf{ identity},h,g\in G,$

  - $h\star g=e\implies h\text{ left inverse of }g$
  - $g\star h=e\implies h\text{ right inverse of }g$

- **P3** two sided inverse

  $\forall e\textbf{ identity},g\in G,\star\textbf{ associative},$

  $(\exist h_1\text{ left inverse of }g,h_2\text{ right inverse of }g)$

  $\implies h_1=h_2=:g^{-1}$ (**two sided inverse**)

- **P4** uniqueness of inverse

  $\forall e\textbf{ identity},g\in G,\star\textbf{ associative},$

  $\exist g^{-1}\implies\exist!g^{-1}$

- ==**D6** group==

  A **group** $(G,\star)$ is a set $G$ together with a binary operation $\star$ (**group operation**) on $G$ such that

  - $\star\textbf{ associative}$
  - $\exist e\textbf{ identity}$
  - $\forall g\in G,\exist g^{-1}\in G$

- **E7**
  
  - $(\Z,+),(\R,+),(\C,+)$ are groups
  - $(\N,+),(\Z,-),(\C,\cdot)$ are not groups 
  - $(\{e,\star:e\star e\mapsto e\}$ is a **trivial group**
  
- ==**D7/D12** orders==

  $\group,$

  - order of group

    - $G$ has exactly $n$ elements
      - $|G|=n$ ($G$ has **order** $n$)
      - $G$ is a **finite group**

    - Otherwise, $(G,\star)$ is an infinite group

  - order of element

    $\forall g\in G,$ **order** of $g$ is the smallest $n\in\N:g^n=e$

- **D8/E9** Abelian group

  $\group,\star\textbf{ commutative}\implies G\textbf{ Abelian group}$

  - $(\{f:\R\to\R\textbf{ invertible}\},\circ)$ is a group with identity $id:x\mapsto x,$ it is not Abelian since $\circ$ is not commutative: $f(g(x))\neq g(f(x))$

- **P5**

  $\group,g,h\in G,$

  - $g\star h=e\lor h\star g=e\implies h=g^{-1}$
  - $(g^{-1})^{-1}=g$

- **P6**

  $\group,g,h\in G:(g\star h)^{-1}=h^{-1}\star g^{-1}$

- **D9/P7** exponent

  $\group,g\in G,m,n\in\Z,$

  $g^n:=\begin{dcases}g\star g\star\cdots\star g&n>0\\g^{-1}\star g^{-1}\star\cdots\star g^{-1}&n<0\\e&n=0\end{dcases}$

  - $g^n\star g^m=g^{n+m}$
  - $(g^n)^m=g^{nm}$

- **D10/P8** congruent modulo

  $\forall a,b,c\in\Z,$

  $a-b\text{ divisible by }n\implies a\equiv b\mod n$ ($a$ **congruent to** $b$ **modulo** $n$)

  - $a\equiv a\mod n$ (*reflexivity*)
  - $a\equiv b\mod n\implies b\equiv a\mod n$ (*symmetry*)
  - $a\equiv b\mod n\land b\equiv c\mod n\implies a\equiv c\mod n$ (*transitivity*)

- **D** equivalence class of modulo

  - $\forall a\in\Z,[a]:=\{b\in\Z,b\equiv a\mod n\}$

  - $\Z_n:=\{[0],[1],\ldots,[n-1]\}$

- **L1**

  $\forall a,a',b,b'\in\Z,[a]=[a']\land[b]=[b'],$

  - $[a+b]=[a'+b']$
  - $[ab]=[a'b']$

- **D** addition and multiplication on $\Z_n$

  - $+:\Z_n\times\Z_n\to\Z_n,([a]_n,[b_n])\mapsto[a+b]_n$
  - $\cdot:\Z_n\times\Z_n\to\Z_n,([a]_n,[b_n])\mapsto[ab]_n$

- **L2**

  $\forall [a]\in\Z_n,$

  $(\exist[b]\in\Z_n:[a][b]=[1])\iff a\text{ coprime to }b$

- **D11**

  $\Z^*_n=\{[a]\in\Z_n|\exist[b]\in\Z_n:[a][b]=1\}$

- **P9/10**
  - $(\Z_n,+)$ **finite Abelian group**

  - $(\Z_n^*,\cdot)$ **finite Abelian group**

    

## 2. Cyclic groups

- **L3** 

  $\group\text{ finite},$

  $\implies\forall g\in G,g$ has finite order

- **L4**

  $\group,g\in G$ with order $n,$

  $e,g,g^2,\ldots,g^{n-1}$ are all different

- **C1**

  $\group,|G|=n,$

  $\implies\forall g\in G,g$ has order at most $n$

- ==**D13/L5** cyclic group==

  $\group,$

  $(\exist g\in G:G=\{g^n|n\in\Z\})\implies G\textbf{ cyclic},g\textbf{ generator}$

  - $\implies G\textbf{ Abelian}$

- **L6**

  $\group\text{ finite with size }n,$

  $G\textbf{ cyclic}\iff\exist g\in G$ of order $n$

- **L7**

  $\group\text{ finite and cyclic},$

  $\exist\text{ at most one }g\in G$ with order 2



## 3. Symmetric groups

- **D14** injection, surjection, bijection

  $\forall f:X\to Y$

  - $\forall x_1,x_2\in X,f(x_1)=f(x_2)\implies x_1=x_2$

    $\implies f\textbf{ injective}$ (one-to-one)

  - $\forall y\in Y,\exist x\in X:f(x)=y$

    $\implies f\textbf{ surjective}$ (onto)

  - $f\text{ injective and surjective}\implies f\textbf{ bijective}$

    $\iff\exist f^{-1}:Y\to X:\forall x(f^{-1}f(x)=x)\land\forall y\in Y(ff^{-1}(y)=y)$

- **D15** permutation

  A **permutation** (on $n$ symbols) is a bijection

  $\sigma:\{1,\ldots,n\}\xrightarrow{\sim}\{1,\ldots,n\}$ (Re-ordering 1 to n)

  - *two-row notation:*

    $\begin{vmatrix}1&2&\cdots&n\\\sigma(1)&\sigma(2)&\cdots&\sigma(n)\end{vmatrix}$

- ==**D16** symmetric group==

  The set (of functions) $S_n=\{\sigma:\{1,\ldots,n\}\xrightarrow{\sim}\{1,\ldots,n\}\}$ of all permutations on $n$ symbols is a **symmetric group** (on $n$ symbols)


- **D17** cycle

  $\forall\sigma\in S_n,$

  $(\exist\text{ distinct }a_1,\dots,a_k\in\{1,\ldots,n\}:$

  $\sigma(a_1)=a_2,\ldots,\sigma(a_i)=a_{i+1},\ldots,\sigma(a_k)=a_1)$

  $\implies\sigma\textbf{ k-cycle}$

- **P11/12/13** group of permutations
  
  - $(S_n,\circ)$ is a group
  - $\# S_n=n!$
  - $\forall\sigma\in S_n\textbf{ k-cycle},\sigma$ has order $k$

- **D18** disjoint cycles

  $(a_1,\ldots,a_k)$ and $(b_1,\ldots,b_m)$ are disjoint if no $a_i$ is equal to any $b_j$

  - Commutative

- **L8**

  - $\forall i\in\{1,\ldots,n\},\exist d\in\Z^+:\sigma^d(i)=i$
    - If $d$ is the smallest such +ive integer, $I=\{i,\sigma(i),\ldots,\sigma^{d-1}(i)\}$ are all distinct
    - $\{1,\ldots,n\}\ni j\notin I\implies\sigma(j)\notin I$

- **P14/E22**

  Any permutation can be expressed as a product of some disjoint cycles

  - $\sigma=\begin{vmatrix}1&2&3&4&5&6&7\\4&1&3&2&6&7&5\end{vmatrix}=(1,4,2)(3)(5,6,7)$

    has **cycle-type** $(3,3)$



## 4. Subgroups

- ==**D19** subgroup==

  $\group,\forall H\sube G,$

  - $e\in H$

  - $\forall g,h\in H, gh\in H$
  - $\forall g\in H,g^{-1}\in H$

  $\implies H\leq G$ (**subgroup**)

- **D20**

  $\group,$

  - $\{e\}\sube G$ **trivial subgroup** (resp. non-trivial)
  - $G'\sub G$ **proper subgroup**

- **P15** subgroup test

  $\group,\forall \empty\neq H\sube G,$

  $(\forall x,y\in H,x\star y^{-1}\in H)\implies H\leq G$

- **D21/L9/10** cyclic subgroup

  $\group,\forall g\in G,$

  $\lang g\rang:=\{g^i:i\in\Z\}\leq G$ (**cyclic subgroup generated by** $g$)

  - $g$ has order $n\implies\lang g\rang$ has order $n$



## 5. Cosets and Lagrange's Theorem

- ==**D22** cosets==

  $\group,H\leq G,g\in G$

  - $gH:=\{g\star h:h\in H\}$ (**left coset** of $H$ by $g$)
  - $Hg:=\{h\star g:h\in H\}$ (**right coset**)

- **P16/C2** cosets are disjoint

  $\group,H\leq G,\forall g_1,g_2\in G,$

  $g_1H=g_2H\iff g_2\in g_1H$

  - $\forall g\in G,g$ lies in exactly one of the left cosets of $H$

  - The left cosets form a **partition** of $G:$

    $G=\bigcup g_iH$

- **L11** all left cosets have the same size

  $\group,\forall H\sub G$ finite subgroup,

  $\forall g\in G,\#gH=\#H$

- **T1/D23** Lagrange Theorem (index)

  $\group,\forall H\leq G,$

  $\#G=\#H\cdot\#(G:H)$ (The order of $H$ divides the order of $G$)

  - $(G:H):=\{gH|g\in G\}$ (the set of all left cosets)

  - $\#(G:H)$ is the **index** of $H$

- **C3/4**

  $\group$ **finite**, $\forall g\in G,$

  - order of $g$ divides $\#G$

  - $\#G\in\mathbb P\implies G$ **cyclic**

- **C5** Fermat's Little Theorem

  $\forall a\in\Z,p\in\mathbb P,$

  $a\not\equiv0\mod{p}\implies a^{p-1}\equiv1\mod{p}$

  

## 6. Normal subgroups and quotient groups $\newcommand{\nmsg}{\trianglelefteq}$

- **D24** normal subgroup

  $\group,H\leq G,$

  $Hg=gH\implies H\nmsg G$ (**normal subgroup**)

- **P17/L12** conjugacy criterion

  $\group,H\leq G,$

  $\#(G:H)=2\implies H\nmsg G\iff\forall g\in G,h\in H,ghg^{-1}\in H$

- **D25** conjugate

  $\group,\forall g,x\in G,$

  - $gxg^{-1}$ is the **conjugate** of $x$ by $g$
  - $c:G\to G,\\x\mapsto gxg^{-1}$ is the **conjugation**

- **T2/D26** conjugacy relation

  $\group,\forall x_1,x_2\in G,$

  Relation $x_1\sim x_2\iff\exist g\in G:x_2=gx_1g^{-1}$ (**conjugacy**)

  - It is an **equivalence relation** on $G$
  - $C_a:=\{gag^{-1}|g\in G\}$ is the **conjugacy class** of $a$

- **E38** conjugacy class of abelian group

  $\group,$

  $G$ **abelian** $\implies$ there are as many conjugacy classes as elements

- **P18/C6**

  $\group,$

  - conjugacy classes are **disjoint**
  - conjugacy classes form a partition of $G$

- **T3**

  $\group,H\leq G,$

  $H\nmsg G\iff\forall$ **conjugacy class** $C_g,$ *either*

  - $C_g\sube H$
  - $C_g\cap H=\empty$

- **D27/P19** conjugate subgroup

  $\group,H\leq G,\forall g\in G,$

  $gHg^{-1}:=\{ghg^{-1}|h\in H\}$ (**conjugate subgroup**)

- **C7** unique conjugate subgroup of normal subgroup

  $\group,H\nmsg G,$

  $H$ itself is the only unique conjugate subgroup to $H$

- **D28/P20** coset multiplication

  $\cdot:(G:H)\times(G:H)\to(G:H),\\(gH,g'H)\mapsto gH\cdot g'H:=gg'H$ (**coset multiplication**)

  - This is well-defined $\iff H\nmsg G$

- **D29/P21** quotient group/factor group

  $\group,H\nmsg G,$

  $G/H:=(G:H,\cdot)$ (**quotient group** of $G$ by $H$) 



## 7. The first Isomorphism Theorem $\newcommand{\groups}{\group,(G',\cdot)}$

- **D30** group homomorphism

  $\groups,\forall g_1,g_2\in G,$

  $f:G\to G',\\f(g_1\star g_2)=f(g_1)\cdot f(g_2)$ (**group homomorphism**)

- **P22** properties of group homomorphism

  $\groups,\textbf{ homomorphism }f:G\to G',$

  - $f(e_G)=e_{G'}$
  - $\forall g\in G,f(g^{-1})=f(g)^{-1}$

- **D31** preimage

  $\forall\text{ sets }S,S',\forall f:S\to S',$

  $f^{-1}(S'):=\{s\in S|f(s)\in S'\}$ (**preimage** of $S'$ under $f$)

- **P23** 

  $\groups,\textbf{ homomorphism }f:G\to G',$

  - $H\leq G\implies f(H)\leq G'$
  - $H'\leq G'\implies f^{-1}(H')\leq G$
  - $H'\nmsg G'\implies f^{-1}(H')\nmsg G$

- **D32** group isomorphism

  A **bijective** homomorphism is a group isomorphism

  $G\cong G'$ (**isomorphic** groups)

- **D33/P25/26** kernel and image as subgroups

  $\forall\textbf{ homomorphism }f:G\to G',$

  - $\ker f=\{g\in G|f(g)=e_{G'}\}\nmsg G$
  - $\text{Im }f=\{g'\in G'|\exist g\in G:f(g)=g'\}\leq G'$

- **P24** injectivity with kernel

  $\forall\textbf{ homomorphism }f:G\to G',$

  $f$ **injective** $\iff\ker f=\{e_G\}$

- **C8**

  $\group,H\leq G,$

  $H\nmsg G\iff\exist(G',\cdot),\exist\textbf{ homomorphism }f:G\to G':\ker f=H$

- **T4** First Isomorphism Theorem

  $\forall\textbf{ homomorphism }f:G\to G',$

  $\text{Im }f\cong G/\ker f$

- **C9**

  $\group\textbf{ finite},\forall\textbf{ homomorphism }f:G\to G',$

  $\implies|\text{Im }f|$ divides $\#G$

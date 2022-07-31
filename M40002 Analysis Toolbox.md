## 1. Logic

- **E1.5** element in infinite union

  $x\in\bigcup^\infin_{n=1}S_n\implies\exist n\in\N,x\in S_n\\$

  

## 2. Numbers

- **A2.1** basic axioms of $\Q$

  1. $a+b=b+a$

  1. $a\times b=b\times a$
  2. $a+(b+c)=(a+b)+c$ 
  3. $a\times(b\times c)=(a\times b)\times c$
  4. $a\times(b+c)=(a\times b)+(a\times c)$
  5. $\exist0\in\Q:\forall a\in\Q,a+0=a$
  6. $\exist1\in\Q:\forall a\in\Q,0\neq1,a\times1=a$
  7. $\forall a\in\Q,\exist(-a)\in\Q:a+(-a)=0$
  8. $\forall a\in\Q\textbackslash\{0\},\exist a^{-1}\in\Q:a\times a^{-1}=1$

- **A2.2** order axioms

  10. $\forall x\in\Q, x>0\textbf{ or }x=0\textbf{ or }-x>0$ **(Trichotomy axiom)**
  11. $x>0,y>0\implies x+y>0$
  12. $x>0,y>0\implies xy>0$
  13.  $\forall x\in\Q,\exist n\in\N:n>x$ **(Archimedean axiom)**

- **E2.3** transitivity of $>$

  $x>y>z\implies x>z$

- **E2.4** trichotomy order

  $\forall a\in\Q,\forall x\in\Q,x>a\textbf{ or }x=a\textbf{ or }x<a$

- **D2.6** periodic decimal to $\Q$

  $a_0.a_1\ldots a_i\overline{a_{i+1}a_{i+2}\ldots a_j}\\=\sum_{k=0}^i\frac{a_k}{10^k}+(\frac{a_{i+1}a_{i+2}\ldots a_j}{10^j})(\frac{1}{1-10^{i-j}})$

- **E2.7** order of periodic decimals

  $a:=a_0.a_1a_2\ldots a_{n-1}a_na_{n+1}\ldots\\b:=a_0.a_1a_2\ldots a_{n-1}b_na_{n+1}\ldots\\a<b\iff a_n<b_n$

- **T2.8** every $\Q$ equals a periodic decimal

  $\forall x\in\Q,x=a_0.a_1\ldots a_i\overline{a_{i+1}a_{i+2}\ldots a_j}$

- **P2.14** different decimal expansions

  $a_0.a_1a_2\ldots a_n\bar{9}=a_0.a_1a_2\ldots(a_n+1)$

- ==**E2.15** density of $\R$==

  $\forall x,y\in\R,x<y,$

  - $\exist z\in\Q:x<z<y$

  - $\exist z\notin\Q:x<z<y$

- ==**D** countability==

  $S$ **countable** $\iff\exist$ **bijection** $f:\N\rightarrow S$

- ==**P2.16** countability of subset of $\N$==

  $S\sub\N$ **infinite** $\implies S$ **countable**

- **P2.17**

  $\Z$ **countable**

- ==**E2.18** countability of union==

  - $A,B$ **countable** $\implies A\cup B$ **countable**
  - $A$ **finite**, $B$ **countable** $\implies A\cup B$ **countable**

- ==**T2.19** zigzag argument==

  $\Q$ **countable**

- ==**T2.21** Cantor's Diagonal Argument==

  $\R$ **uncountable**

- **P1Q1** countability of infinite union

  $S_n$ **disjoint and countable** $\implies \bigcup^\infin_{n=1}S_n\\$ **countable**

- **P1Q2** countability of Cartesian product
  - $S,T$ **countable** $\implies S\times T$ **countable**
  - $S$ **countable** $\implies \bigcup^\infin_{n=1} S^n\\$ **countable**

- **P1Q3** countability of algebraic and transcendental
  - $\mathbb{A}$ **countable**
  - $\R\textbackslash\{\mathbb{A}\}$ **uncountable**

- **P1Q4** countability of power set of $\N$

  $\mathcal{P}(\N)$ **uncountable**

- **P1Q5** countability of set of finite subsets of $\N$

  $\{S\textbf{ finite }|S\in\mathcal{P}(\N)\}$ **countable**

- **D** maximum/minimum 

  $\forall x\in S\sub\R,$

  - $x=\max(S)\iff\forall s\in S,x\geq s$

  - $x=\min(S)\iff\forall s\in S,x\leq s$

- **E2.22** uniqueness of maximum and existence of minimum

  $\forall S\sub\R,$

  - $\exist\max(S)\implies\exist!\max(S)$

  - $\exist\max(S)\implies\exist\min(-S:=\{-s|s\in S\})=-\max(S)$

- **D** bound

  $\forall \empty\neq S\sub\R,$

  - $S$ **bounded above** $\iff\exist b\in\R:\forall s\in S,s\leq b$
  - $S$ **bounded below** $\iff\exist b\in\R:\forall s\in S,b\leq s$
  - $S$ **bounded** $\iff$ $S$ **bounded above** $\and S$ **bounded below**

- **E2.24** bounded equidistantly

  $S$ **bounded** $\iff\exist k>0:\forall s\in S,|s|\leq k$

- ==**D** supremum/infimum==

  $\forall \empty\neq S\in\R,\forall x\in\R,$

  - $x=\sup(S)\iff x$ **upper bound** $S\and\forall y$ **upper bound** $S, x\leq y$
  - $x=\inf(S)\iff x$ **lower bound** $S\and\forall y$ **lower bound** $S, x\geq y$

- **E2.26/2.28** uniqueness of supremum and existence of infimum

  $\forall \empty\neq S\in\R,$

  - $\exist\sup(S)\implies\exist!\sup(S)$
  - $\exist\sup(S)\implies\exist\inf(-S:=\{-s|s\in S\})=-\sup(S)$

- ==**E2.30** maximum and supremum==

  $\sup(S)\in S\iff\exist\max(S)=\sup(S)$

- ==**T2.31** Completeness Axiom of $\R$==

  $\empty\neq S\sub\R$ **bounded above** $\implies\exist\sup(S) $

- **E2.33**

  $\empty\neq S\sub\R$ **bounded below** $\implies\exist\inf(S)$​

- **P2.38** least upper bound

  $\forall \empty\neq S\in\R,\forall x$ **upper bound** $S,$

  $x=\sup(S)\iff\forall\epsilon>0,\exist s\in S:s>x-\epsilon$

- **T2.44/P2Q6** triangular inequalities

  $\forall x,y\in\R,$

  - ==$|x+y|\leq|x|+|y|$==
  - $|x+y|\geq|x|-|y|$
  - $|x+y|\geq|y|-|x|$
  - $|x-y|\geq\left||x|-|y|\right|$
  - $|x|\leq|y|+|x-y|$
  - $|x|\geq|y|-|x-y|$
  - $|x-y|\leq|x-z|+|y-z|$

- **E2.46** limit

  $\forall\epsilon>0,|x-a|<\epsilon\iff x=a$

- **P2Q1** supremum statements
  - $S\sub\Z\implies\sup(S)\in\Z$
  - $\sup(S)=\inf(\R\textbackslash S)\iff \exist a\in\R,S\in\{(-\infin,a),(-\infin,a]\}$

- **P2Q2** supremum of infinite union

  $\forall n\in\N,S_n\sub\R\implies\sup\{\sup(S_1),\sup(S_2),\ldots\}=\sup(\bigcup^\infin_{n=1}S_n)$

- **P2Q3** supremum of set addition

  $\forall S,T\sub\R,\sup(S+T:=\{s+t|s\in S,t\in T\})=\sup(S)+\sup(T)$



## 3. Sequences

- **D** sequence

  A sequence is a function $a:\N\rightarrow\R,$ which can be described as

  - **list** $1,0,1,0,\ldots$
  - **closed formula** $a_n=\frac{1-(-1)^n}{2}\\$
  - **recursion** $a_1=a_2=1,a_n=a_{n-1}+a_{n-2}$ for $n\geq 3$
  - **summation** $a_n=\sum^n_{i=1}b_i\\$ (**series**)

- **E3.2** all sequences can be written as series

  $\forall(a_n),\exist(b_n),a_n=\sum^n_{i=1}b_i\\$

- ==**D** convergence==

  - $\forall\epsilon>0,\exist N\in\N:\forall n\geq N,|a_n-a|<\epsilon\iff a_n\rightarrow a$ (as $n\rightarrow\infin$) 

    To prove $a_n\rightarrow a:$

    - Fix (arbitrary) $\epsilon>0$
    - Calculate $|a_n-a|$ and find a good estimate $b_n\geq|a_n-a|$
    - Try to solve $b_n<\epsilon$ and find $N\in\N:\forall n\geq N,b_n<\epsilon$
    - Put everything together

  - $a_n$ **converges** $\iff\exist a:\forall\epsilon>0,\exist N\in\N:\forall n\geq N,|a_n-a|<\epsilon$

  - $a_n$ **diverges** $\iff\forall a,\exist\epsilon>0:\forall N\in\N,\exist n\geq N:|a_n-a|\geq\epsilon$

- **T3.14** uniqueness of limits

  $a_n\rightarrow a\land a_n\rightarrow b\implies a=b$

- ==**D/P3Q2** diverges to infinity==

  $\forall R>0,\exist N\in\N:\forall n\geq N,a_n>R\iff a_n\rightarrow+\infin$ (as $n\rightarrow\infin$) 

- **P3Q3** convergence after replacing finite terms

  $a_n\rightarrow a,(b_n):\{n\in\N|a_n\neq b_n\}$ is finite $\implies b_n\rightarrow a$ 

- **P3Q4** existence of sequence converging to supremum

  $\forall\empty\neq S\sub\R$ **bounded above**, $\exist(s_n)\in S:s_n\rightarrow\sup(S)$

- **P3.16** convergence and bounded

  $a_n$ **converges** $\implies\exist A\in\R,\forall n\in\N,|a_n|\leq A$ (**bounded**)

- ==**T3.19/P4Q5** algebra of limits==

  $a_n\rightarrow a$ and $b_n\rightarrow b,$

  - $a_n+b_n\rightarrow a+b$
  - $a_nb_n\rightarrow ab$
  - $b\neq0\implies\frac{a_n}{b_n}\rightarrow\frac a b\\$

- **T3.21** convergence of bounded monotone sequence

  - $(a_n)$ **bounded above** and $\forall n\in\N,a_{n+1}\geq a_n$

    $\implies a_n\rightarrow a:=\sup\{a_i|i\in\N\}\Leftrightarrow a_n\uparrow a$

  - $(a_n)$ **bounded below** and $\forall n\in\N,a_{n+1}\leq a_n$

    $\implies a_n\rightarrow a:=\inf\{a_i|i\in\N\}\Leftrightarrow a_n\downarrow a$

- **E3.22** order of convergence

  $a_n\rightarrow a$ and $b_n\rightarrow b,$ $(\forall n\in\N,a_n\leq b_n)\implies a\leq b$

- **E3.23/P5Q2** ratio test

  $|\frac{a_{n+1}}{a_n}|\rightarrow L\\$ ($\lim_{n\rightarrow\infin}|\frac{a_{n+1}}{a_n}|=L\\$),

  - $L<1\implies \sum^\infin_{n=1}a_n\\$ **converges**, $a_n\rightarrow 0$
  - $L> 1\implies\sum^\infin_{n=1}a_n\\$ **diverges**, $|a_n|\rightarrow\infin$

- ==**D** Cauchy sequence==

  $\forall\epsilon>0,\exist N\in\N:\forall n,m\geq N,|a_n-a_m|<\epsilon\iff(a_n)$ **Cauchy**

- ==**P3.25/T3.27/C3.28** convergence and Cauchy==

  $(a_n)$ **convergent** $\iff(a_n)$ **Cauchy**

- **L3.26** Cauchy and bounded

  $(a_n)$ **Cauchy** $\implies(a_n)$ **bounded**

- **P4Q2** convergence of complex sequence

  $\forall(a_n)\in\C,a_n\rightarrow a+ib\in\C\iff Re(a_n)\rightarrow a\land Im(a_n)\rightarrow b$

- **P4Q3** squeezing convergence

  $a_n\rightarrow a$ and $c_n\rightarrow a,$ $(\forall n\in\N,a_n\leq b_n\leq c_n)\implies b_n\rightarrow a$

- **P4Q4** product convergence to zero

  $(b_n)$ **bounded** $\land a_n\rightarrow 0\implies a_nb_n\rightarrow 0$

- **D/E3.32** subsequence

  $b_i=a_{n(i)}\forall i\in\N$ is a **subsequence** of $(a_n)$

  - $n:\N\rightarrow\N,i\mapsto n(i)$ is strictly monotonically increasing
  - $\forall i\in\N,n(i)\geq i$

- ==**T3.34** Bolzano-Weierstrass==

  $(a_n)$ **bounded** $\implies\exist$ **convergent subsequence**

- **P3.39** subsequences of convergent sequence

  $a_n\rightarrow a\implies\forall b_i=a_{n(i)}$ **subsequence**, $b_i\rightarrow a$ (as $i\rightarrow\infin$)

- ==**L3.40** convergence definition with $c\epsilon$==

  $\forall c>0,(a_n\rightarrow a\iff \forall\epsilon>0,\exist N\in\N:\forall n\geq N,|a_n-a|<c\epsilon)$

- **E3.42** reciprocal of positive sequence converging to zero

  $\forall(a_n)>0,(a_n\rightarrow 0\iff\frac{1}{a_n}\rightarrow+\infin)\\$



## 4. Series

- **D** (infinite) series and partial sums

  $\forall (a_i),$

  - $\sum^\infin_{n=1}a_n\\$ is the formal expression of the series
  - $s_n:=\sum^n_{i=1}a_i\\$ is the sequence of partial sums
  - $a_n=s_n-s_{n-1}$

- **D** convergence of series

  $\sum^\infin_{n=1} a_n=A\iff s_n\rightarrow A\\$

- **T4.2** necessary condition for series convergence

  $\sum^\infin_{n=1}a_n\\$ **converges** $\implies a_n\rightarrow0$ 

- **P4.6** monotone increasing series

  $\forall(a_n)\geq 0$ ($s_n$ monotonically increasing),

  - $\sum^\infin_{n=1}a_n\\$ **converges** $\iff(s_n)$ **bounded above**
  - $\sum^\infin_{n=1}a_n\rightarrow+\infin\iff(s_n)\\$ **unbounded**

- ==**T4.7** comparison test==

  $\forall0\leq a_n\leq b_n$,

  - $\sum b_n$ **converges** $\implies\sum a_n$ **converges**
  - $0\leq\sum^\infin_{n=1}a_n\leq\sum^\infin_{n=1}b_n\\$

- **E4.8** comparison test converse

  $\forall0\leq a_n\leq b_n,\sum a_n\rightarrow+\infin\implies\sum b_n\rightarrow+\infin$

- **E4.10**

  $\forall\alpha>1,\sum^\infin_{n=1}\frac{1}{n^\alpha}\\$ **converges**

- **P5Q1** convergence of powers

  - $r\in(0,1)\implies r^n\rightarrow 0$
  - $r\in(1,\infin)\implies r^n\rightarrow\infin$

- **P5Q3** reciprocal of positive sequence converging to non-zero

  $\forall(a_n)>0,(a_n\rightarrow a\neq0\implies\frac{1}{a_n}\\$ **bounded**$)$

- **P5Q5** existence of special subsequence

  $\forall(a_n),\exist b_i=a_{n(i)}$ **subsequence**, $b_i\rightarrow0\textbf{ or }b_i\rightarrow+\infin\textbf{ or }b_i\rightarrow-\infin$

- **T4.11** algebra of limits of series

  $\sum a_n,\sum b_n$ **convergent** $\implies\sum^\infin_{n=1}(\lambda a_n+\mu b_n)=\lambda\sum^\infin_{n=1}a_n+\mu\sum^\infin_{n=1}b_n\\$

- ==**D** absolute convergence==

  $\forall(a_n)\in\R,$ (or $\in\C$)

  $\sum^\infin_{n=1}a_n\\$ **absolutely convergent** $\iff\sum^\infin_{n=1}|a_n|\\$ **convergent**

- **T4.14** absolute convergence implies convergence

  $\forall(a_n)\in\R,$ (or $\in\C$)

  $\sum a_n$ **absolutely convergent** $\implies\sum a_n$ **convergent**

- **T4.16** sandwich test

  $\forall c_n\leq a_n\leq b_n,$

  $\sum c_n,\sum b_n$ **convergent** $\implies\sum a_n$ **convergent**

- ==**T4.17/P7Q1** fractional comparison test==

  $\forall\frac{a_n}{b_n}\to L\in R,\\$

  $\sum b_n$ **absolutely convergent** $\implies\sum a_n$ **absolutely convergennt**

- **E4.19** tail determines convergence

  $\forall N\in\N,(a_n)\in\R,$

  $\sum^\infin_{n=1}a_n\\$ **converges** $\iff\sum^\infin_{n=N}a_n\\$ **converges**

- ==**T4.20** alternating series test==

  $\forall(a_n)$ **alternating**, $|a_n|\downarrow0\implies\sum a_n$ **converges**

- ==**T4.23** ratio test==

  $\forall(a_n)\in\R,$ (or $\in\C$)

  $|\frac{a_{n+1}}{a_n}|\to r<1\implies\sum a_n$ **absolutely convergent**

- ==**T4.26** root test==

  $\forall(a_n)\in\R,$ (or $\in\C$)

  $|a_n|^\frac1 n\to r<1\implies\sum a_n$ **absolutely convergent**

- **D** rearrangement of sequence

  $\forall n:\N\to\N$ **bijection**,

  $b_i:=a_{n(i)}$ is a **rearrangement** (or reordering) of $(a_n)$

- **E4.31** arbitrary convergence of rearrangement

  $\forall(a_n),\begin{dcases}a_n\to0\\\sum_{n:a_n\geq0}a_n\to+\infin\\\sum_{n:a_n\leq0}a_n\to-\infin\end{dcases}\implies\forall k\in\R,$

  $\exist(b_m)$ **rearrangement:** $b_m\to k$

  *Method:*

  - Add non-negative terms until partial sum $>k$
  - Add negative terms until partial sum $<k$
  - Repeat

- **T4.34** necessary conditions for absolute convergence

  $\sum a_n$ **absolutely convergent** $\iff[1]\land[2]\implies[3]\land[4]$ where

  - $\text{[1] }\sum_{n:a_n\geq0}a_n\uparrow A\\$
  - $\text{[2] }\sum_{n:a_n<0}a_n\downarrow B\\$
  - $\text{[3] }\sum a_n=A+B$
  - $\text{[4] }\forall b_m$ **rearrangement**, $\sum b_m=A+B$

- ==**T4.35** radius of convergence==

  $\forall z\in\C,(a_n)\in\R$ (or $\in\C$), $\exist R\in[0,\infin]:$

  - $|z|<R\implies\sum a_nz^n$ **absolutely convergent**
  - $|z|>R\implies\sum a_nz^n$ **divergent**
  - Indeterminate at $|z|=R$

  $R=\sup\{r\in[0,\infin)|\lim_{n\to\infin}a_nr^n=0\}\\$

- ==**E4.38** testing radius of convergence==

  $\forall(a_n)\in\R,$ (or $\in\C$)

  $|\frac{a_{n+1}}{a_n}|\to a\in[0,\infin]\implies R=\frac1a\\$ is radius of convergence of $\sum a_nz^n$

- **D** Cauchy product

  $\forall (a_n),(b_n)\in\R,c_n:=\sum^n_{i=0}a_ib_{n-i}\\$

  $\sum c_n$ is the **Cauchy product** of $\sum a_n,\sum b_n$

- **T4.39** convergence of Cauchy product

  $\forall (a_n),(b_n)\in\R,$

  $\sum a_n,\sum b_n$ **absolutely convergent** $\implies\sum c_n$ (**Cauchy product**) **absolutely convergent** to $(\sum a_n)\cdot(\sum b_n)$

- **C4.40** radius of convergence of Cauchy product

  $\forall(a_n),(b_n)\in\R,$

  $\sum a_nz^n,\sum b_nz^n$ have $R_A,R_B\implies\sum c_nz^n$ (**Cauchy product**) has $R_C\geq\min\{R_A,R_B\}$

- **E4.41**

  $\forall a,b\in\R,$

  $(x<a\implies x\leq b)\implies a\leq b$

- **E4.42** power series of 1

  $\sum z^n$ has $R_A=1$

- **P6Q2**

  - $\forall r>1,\frac n{r^n}\to0\\$
  - $n^\frac1n\to1$

- **P6Q3**

  - $\forall M\in\R,\frac{M^n}{n!}\to0\\$
  - $n!^\frac1n$ **unbounded**

- **P6Q4** equivalent definition for existing convergent subsequence

  $\exist a\in\R:\forall\epsilon>0,N\in\N,\exist n\geq\N:|a_n-a|<\epsilon$

- **P6Q7** multiple of convergent sequence

  $\forall c\in\R,\sum a_n\to a\implies\sum ca_n\to ca$

- **P6Q9** polynomial vs exponential

  $\forall a,b\in\R,\sum^\infin_{n=1}\frac{n^a}{b^n}\begin{dcases}\textbf{converges}&|b|>1\\\textbf{diverges}&|b|<1\end{dcases}$

- ==**D** exponential power series==

  $\forall z\in\C,E(z):=\sum^\infin_{n=0}\frac{z^n}{n!}\\$ **absolutely convergent**

- **P4.43** algebra of EPS

  $E(z)E(w)=E(z+w)$

- **C4.44** reciprocal of EPS

  $E(z)\neq 0\land\frac1{E(z)}=E(-z)\\$

- **D** Euler's number

  $e:=E(1)$

- **C4.45/P4.46** EPS and exp

  $\forall x\in\N(\Q;\R),E(x)=e^x$

- **P4.47** properties of EPS

  $\forall x\in\R,$

  - $E(x)>0$
  - $x\geq0\implies E(x)\geq1\land x>0\implies E(x)>1$
  - $E(x)$ **strictly increasing**
  - $\forall|x|<1,|E(x)-1|\leq\frac{|x|}{1-|x|}\\$
  - $x\mapsto E(x)$ **continuous bijection** $\equiv\R\to(0,\infin)$

- **E4.49** trigonometric functions
  - $\cos\theta:=Re(E(i\theta))$
  - $\sin\theta:=Im(E(i\theta))$



## 5. Continuity

- ==**D** limit==

  $\lim_{x\to a}f(x)=b\iff\\\forall\epsilon>0,\exist\delta>0:0<|x-a|<\delta\implies|f(x)-b|<\epsilon$

- **E5.2** uniqueness of limit

  $(\lim_{x\to a}f(x)=b\land\lim_{x\to a}f(x)=c)\implies b=c\\$

- **D/T5.3** continuity

  $(\forall f:\R\to\R,a\in\R),f$ **continuous** at $a$

  - $\iff\lim_{x\to a}f(x)=f(a)\\$
  - ==$\iff\forall\epsilon>0,\exist\delta>0:|x-a|<\delta\implies|f(x)-f(a)|<\epsilon$==

- **P5.10** continuity of EPS

  $E:\C\to\C,E(z):=\sum^\infin_{n=0}\frac{z^n}{n!}\\$ **continuous** on $\C$

- **P7Q8** 

  $\forall(a_n)\geq0,\sum a_n\textbf{ converges}\iff\sum\frac{a_n}{1+a_n}\textbf{ converges}$

- ==**T1.1** sequential continuity==

  $f:\R\to\R\textbf{ continuous}\text{ at }a\in\R\iff$

  $\forall(x_n)\to a,f(x_n)\to f(a)$

- **P1.2** algebra of continuity

  $\forall f,g:\R\to\R$ **continuous** at $a\in\R,$

  - $f+g,f-g,f\cdot g$ **continuous** at $a$
  - $g(a)\neq0\implies\frac f g\\$ **continuous** at $a$

- **P1.3** continuity of composition

  $\forall f:\R\to\R$ **continuous** at $a,$ $g:\R\to\R$ **continuous** at $f(a),$

  $\implies g\circ f$ **continuous** at $a$

- ==**T1.6** intermediate value theorem==

  $\forall f:[a,b]\to\R$ **continuous**, $c\in[f(a),f(b)],$

  $\exist x\in[a,b]:f(x)=c$

- **P1.7** fundamental theorem of algebra (weak)

  $\forall\text{ polynomial }p(x)$ of odd degree, $p(x)$ has a root

- **P1.8** fixed point

  $\forall f:[0,1]\to[0,1]$ **continuous**,

  $\exist x\in[0,1]:f(x)=x$ (**fixed point**)

- **T1.13** continuity within a closed interval

  $\forall f:[a,b]\to\R,$

  $f\textbf{ continuous}\implies f\textbf{ bounded}$

- ==**T1.14** extreme value theorem==

  $\forall f:[a,b]\to\R$ **continuous**,

  - $\exist c,d\in[a,b]:\forall x\in[a,b],f(c)\leq f(x)\leq f(d)$
  - $\exist c,d\in[a,b]:f(c)=\inf_{x\in[a,b]}f(x),f(d)=\sup_{x\in[a,b]}f(x)\\$

- **P1.15** 

  $\forall f:[a,b]\to\R$ **continuous**,

  $\exist c,d\in[a,b]:\text{Image of }f([a,b])=[f(c),f(d)]$

- **P1.16**

  $\forall f:[a,b](\text{or }\R)\to\R$ **continuous**,

  $f\textbf{ injective}\iff f\textbf{ strictly monotonic}$

- **T1.17**

  $\forall f:\R\to\R$ **continuous** and **injective**,

  $\implies f^{-1}:\R\to\R$ **continuous**

- ==**D/E1.19** open set==

  $\forall S\sub\R,S\textbf{ open}\iff\forall x\in S,\exist\delta>0:(x-\delta,x+\delta)\sub S$

  - $\forall a,b\in\R,(a,b)\textbf{ open}$

- **P1.20** union of open sets

  $\forall\{S_\alpha\}\sub\R$ (finite or not) collection of **open** sets,

  $S=\bigcup_\alpha S_\alpha\\$ **open**

- **P1.21** intersection of open sets

  $\forall S_1,\ldots,S_n\sub\R$ **open**,

  $S=\bigcap_{i=1}^nS_i\\$ **open**

- **P1Q1** 

  $\forall f:\R\to\R\textbf{ continuous},$

  $f(\R)\sub\Q\implies f\textbf{ constant}$

- **P1Q2**

  $\forall f,g:\R\to\R\textbf{ continuous},$

  $\forall x\in\Q,f(x)=g(x)\iff\forall x\in\R,f(x)=g(x)$

- **P1Q6**

  $\forall S\sub\R,d_s(x):=\inf_{s\in S}|x-s|\textbf{ continuous}\\$

- **P1Q7**

  $\forall f:\R\to\R\textbf{ monotonically increasing},\forall x\in\R,$

  - $\sup_{y<x}f(y)=\inf_{y>x}f(y)\iff f\textbf{ continuous}\text{ at }x\\$
  - $\{x\in\R|f\textbf{ discontinuous}\text{ at }x\}$ is at most **countable**

- **P1Q8**

  $\forall f:\R\to\R,f\textbf{ continuous}\iff$

  $\forall U\sub\R\textbf{ open},f^{-1}(U)=\{x\in\R|f(x)\in U\}\textbf{ open}$

- ==**D/E1.23** closed and compact set==

  $\forall S\sub\R,$

  $S\textbf{ closed}\iff\forall\text{sequence }(x_n)\sub S,x_n\to x\in\R\implies x\in S$

  $S\textbf{ compact}\iff S\textbf{ closed and bounded}$

  - $\forall a,b\in\R,[a,b]\textbf{ compact}$
  - $(0,1]$ Neither open nor closed
  - $\R$ both open and closed
  - $\empty$ both open and closed

- **P1.24** complement of open set

  $\forall S\sub\R,S\textbf{ open}\iff T=\R\backslash S\textbf{ closed}$

- **P1.25** union and intersection of closed sets

  - A union of *finitely many* **closed** sets is closed
  - An intersection of *arbitrarily many* **closed** sets is closed

- **P1.26**

  $\forall S\sub\R,S\textbf{ compact}\iff$

  $\forall\text{ sequence }(x_n)\sub S,(x_n)$ has a **convergent subsequece** $x_{n_i}\to x\in S$

- ==**D** uniform continuity==

  $\forall f:S\to\R,f\textbf{ uniformly continuous}\iff$

  $\forall\epsilon>0,\exist\delta>0:\forall x,y\in S,|x-y|<\delta\implies|f(x)-f(y)|<\epsilon$

- **P1.28** uniform continuity and continuity

  $\forall f:S\to\R,f\textbf{ uniformly continuous}\implies f\textbf{ continuous}$

- **P1.32**

  $\forall S\textbf{ compact},f:S\to\R\textbf{ continuous},$

  $\implies f\textbf{ uniformly continuous}$

- ==**D/T1.34** convergence of function sequence==

  $\forall S\sub\R,f_1,f_2,\cdots:S\to\R,$

  - $\forall x\in S,\forall\epsilon>0,\exist N\in\N:n\geq N\implies|f_n(x)-f(x)|<\epsilon$

    $\implies f_n$ converges **pointwise** to $f:S\to\R$

  - $\forall\epsilon>0,\exist N\in\N:\forall x\in S,n\geq N\implies|f_n(x)-f(x)|<\epsilon$

    $\implies f_n$ converges **uniformly** to $f:S\to\R$

    - $\implies f$ **continuous**
    - $f_n\textbf{ uniformly continuous}\implies f\textbf{ uniformly continuous}$

- **C1.35**

  $\forall f_n:S\to\R$ **uniformly convergent sequence of continuous functions**,

  $(\exist\delta>0,a\in S:(a-\delta,a+\delta)\sub S)\implies$

  $\lim_{n\to\infin}\lim_{x\to a}f_n(x)=\lim_{x\to a}\lim_{n\to\infin}f_n(x)\\$

- **T1.36** Weierstrass M-test

  $\forall S\sub\R,f_1,f_2,\cdots:S\to\R$ **continuous**,

  $(\exist M_1,M_2,\cdots:\forall i,\forall x\in S,|f_i(x)|\leq M_i)\implies$

  $(\sum^\infin_{i=1}M_i\textbf{ converges}\implies\sum^\infin_{i=1}f_i(x)\textbf{ converges uniformly to }g:S\to\R\textbf{ continuous})\\$

- **T1.38**

  $\forall f(x)=\sum^\infin_{i=0}a_ix^i\\$ with radius of convergence $R>0,$

  $\implies f\text{ continuous on }(-R,R)$

- **P2Q2**

  $\forall f:\R\to\R\textbf{ continuous},\forall c\in\R,$

  $f^{-1}(c):=\{x\in\R|f(x)=c\}\textbf{ closed}$

- **P2Q3**

  $\forall(S_n)$ where $S_1\supset S_2\supset\ldots,$

  $S_n$ **compact** $\forall n\implies S:=\bigcap^\infin_{n=1}S_n\neq\empty\\$

- **P2Q4**

  $\forall f:\R\to\R\textbf{ continuous},S\sub\R,$

  $S\textbf{ compact}\implies f(S)\textbf{ compact}$



## 2. Differentiation

- ==**D** differentiability==

  $\forall f:\R\to\R,$

  $f\textbf{ differentiable}\text{ at }a\in\R\text{ with derivative }f'(a)\in\R\iff$

  $\exist f'(a)=\lim_{x\to a}\frac{f(x)-f(a)}{x-a}\iff\\$

  $\forall\epsilon>0,\exist\delta>0:|x-a|<\delta\implies\left|\frac{f(x)-f(a)}{x-a}-f'(a)\right|<\epsilon\\$

- **P2.3**

  $\frac{x^n-a^n}{x-a}=\sum_{i=0}^{n-1}x^{n-1-i}a^i=x^{n-1}+x^{n-2}a+\dots+xa^{n-2}+a^{n-1}\\$

- **P2.5** differentiability implies continuity

  $f\textbf{ differentiable}\text{ at }a\in\R\implies f\textbf{ continuous}\text{ at }a\in\R$

- **P2.9/T2.11** quotient rule

  - $\frac d{dx}\frac1{f(x)}=-\frac{f'(x)}{f(x)^2}\\$

  - $\frac d{dx}\frac{f(x)}{g(x)}=\frac{f'(x)g(x)-f(x)g'(x)}{g(x)^2}\\$

- **D** local minimum

  $\forall f:S\to\R,f$ has a **local minimum** at $x\in S\iff$

  $\exist\delta>0:|y-x|<\delta\implies f(y)\geq f(x)$

- **T2.15** Rolle's theorem

  $\forall f\textbf{ continuous}\text{ on }[a,b],\textbf{differentiable}\text{ on }(a,b),$

  $f(a)=f(b)\implies\exist c\in(a,b):f'(c)=0$

- ==**T2.16** mean value theorem==

  $\forall f\textbf{ continuous}\text{ on }[a,b],\textbf{differentiable}\text{ on }(a,b),$

  $\exist c\in(a,b):f'(c)=\frac{f(b)-f(a)}{b-a}\\$

- **P2.17/2.18** sign of derivative

  $\forall f\textbf{ continuous}\text{ on }[a,b],\textbf{differentiable}\text{ on }(a,b),$

  - $(\forall x\in(a,b),f'(x)\geq0)\implies f\textbf{ monotone increasing}\text{ on }[a,b]$

  - $(\forall x\in(a,b),f'(x)=0)\implies f\textbf{ constant}\text{ on }[a,b]$

- **P2.19**

  $\forall f,g\textbf{ continuous}\text{ on }[a,b],\textbf{differentiable}\text{ on }(a,b),$

  $(\forall x\in(a,b),f'(x)=g'(x))\implies\exist c\in\R:\forall x\in[a,b],f(x)=g(x)+c$

- **P2.21**

  $\forall f,g\textbf{ differentiable}\text{ on }(a,b),$

  $\exist c\in(a,b):(f(b)-f(a))g'(c)=(g(b)-g(a))f'(c)$

- ==**T2.22** L'Hopital's rule==

  $\forall f,g\textbf{ differentiable}\text{ on }(c,d)\text{ except possibly at }a\in(c,d),$

  $g'(x)\neq0\text{ on }(c,d)\backslash\{a\},$

  $\lim_{x\to a}f(x)=\lim_{x\to a}g(x)=0\land\lim_{x\to a}\frac{f'(x)}{g'(x)}=L\implies\lim_{x\to a}\frac{f(x)}{g(x)}=L\\$ 

- **P2.25** second derivative

  $\forall f''(x)\text{ exists on a neighbourhood of, and is continuous at } x=a,$

  $f''(a)=\lim_{h\to0}\frac{f(a+h)-2f(a)+f(a-h)}{h^2}\\$

- ==**T2.26** Taylor's theorem==

  $\forall f:[c,d]\to\R\text{ with continuous derivatives }f^{(i)}(x)\forall i\leq n$ and that $f^{(n+1)}(x)\text{ exists }\forall x\in(c,d),$

  - $\forall a\in[c,d],P_n(x):=\sum^n_{i=0}\frac{f^{(i)}(a)}{i!}(x-a)^i\\$ (**Taylor polynomial** of order $n$ at $x=a$)

  - $\forall b\in[c,d],b\neq a,$

    $\exist t\in(a,b):f(b)=P_n(b)+\frac{f^{(n+1)}(t)}{(n+1)!}(b-a)^{n+1}\\$

- ==**D** Taylor series==

  $\forall f^{(n)}(a)\text{ exists }\forall n\geq 0,$

  $\sum^\infin_{n=0}\frac{f^{(n)}(a)}{n!}(x-a)^n\\$ (**Taylor series** for $f$ at $x=a$)

- **P4Q3** log and harmonic sum

  Let $H_n:=\sum^n_{k=1}\frac1k$

  - $\forall n\in\N,\frac1{n+1}<\log(n+1)-\log(n)<\frac1n$
  - $\forall n\geq2,H_n-1<\log n<H_{n-1}$
  - $(H_n-\log n)$ is decreasing sequence, and $\exist\lim_{n\to\infin}(H_n-\log n)$

- ==**D** convexity==

  $\forall f:[a,b]\to\R,$

  $\forall c<t<d\in[a,b],f(c)+\frac{f(d)-f(c)}{d-c}(t-c)\geq f(t)\implies f\textbf{ convex}\\$

- ==**D** convexity alternatives==

  - The height of line through $(c,f(c))$ and $(d,f(d))$ at $x=t$ is at least $f(t)$

  - Consider $S:=\{(x,y)|x\in[a,b],y\geq f(x)\}$

    The line segment between any two points in $S$ lies entirely in $S$

  - Let $t:=sc+(1-s)d$ for some $s\in[0,1],$

    $f$ **convex** $\iff\forall c<d\in[a,b],\forall s\in(0,1),$

    $sf(c)+(1-s)f(d)\geq f(sc+(1-s)d)$

- **P2.34** convexity from second derivative

  $\forall f:[a,b]\to\R\textbf{ continuous},$

  $f\textbf{ convex}\iff\forall x\in(a,b),f''(x)\geq0$

- ==**P5Q1** some inequalities==

  $\forall a,b>0,$

  - $\frac{a+b}2\geq\sqrt{ab}\\$
  - $\forall s\in[0,1],as+b(1-s)\geq a^sb^{1-s}$
  - $\forall x,y\geq0,\frac1a+\frac1b=1\implies\frac{x^a}a+\frac{y^b}b\geq xy\\$

- **T2.36**

  $\forall f_n:[a,b]\to\R\textbf{ differentiable},$

  $(f'_n(x))\text{ converges uniformly on }[a,b]\implies$

  - $(f_n)\text{ converges uniformly to some }f:[a,b]\to\R$
  - $\forall x\in(a,b),f'(x)=\lim_{n\to\infin}f'_n(x)\\$

- **T2.37** differentiation of power series

  $\forall f(x)=\sum^\infin_{n=0}a_nx^n\\$ with radius of convergence $R>0,$

  $\implies f'(x)=\sum^\infin_{n=1}na_nx^{n-1}\space\forall|x|<\R$



## 3. Integration

- ==**D** partition==

  A partition of $[a,b]$ is a finite sequence of numbers $\in\R:$

  $P=(x_0,\ldots,x_k)$ s.t. $a=x_0<\cdots<x_k=b$

  - can be viewed as closed intervals $[x_0,x_1],\ldots,[x_{k-1},x_k]$
  - $\Delta x_i:=x_{i+1}-x_i>0$
  - $\forall f:[a,b]\to\R\textbf{ bounded},$
    - $m_i:=\inf_{x_i\leq t\leq x_{i+1}}f(t)\\$
    - $M_i=\sup_{x_i\leq t\leq x_{i+1}}f(t)\\$

- ==**D** Darboux sum==

  - $L(f,P)=\sum^{k-1}_{i=0}m_i\Delta x_i\\$ (**lower Darboux sum**)
  - $U(f,P)=\sum^{k-1}_{i=0}M_i\Delta x_i\\$ (**upper Darboux sum**)

- **L3.4**

  $\forall f:[a,b]\to\R, P\text{ partition of }[a,b],$

  $\implies L(f,P)\leq U(f,P)$

- **D** refinement

  $\forall P,Q,R\text{ partitions},$

  - Every point of $P$ is a point of $Q\iff P\prec Q$ (is a refinement of $P$)

  - Points in $R$ are precisely those in $P,Q$

    $\iff R$ **common refinement** of $P,Q$

    $\implies P\prec R\land Q\prec R$

- **P3.5**

  $P\prec Q\implies L(f,P)\leq L(f,Q)\leq U(f,Q)\leq U(f,P)$

- **P3.6**

  $\forall f:[a,b]\to\R\textbf{ bounded},P,Q\text{ partitions of }[a,b],$

  $\implies L(f,P)\leq U(f,Q)$

- ==**D** Darboux integrals==

  $\forall f:[a,b]\to\R\textbf{ bounded},$

  - $\underline{\int^b_a}f(x)dx:=\sup_P L(f,P)\\$ (lower Darboux integral)
  - $\overline{\int^b_a}f(x)dx:=\inf_PU(f,P)\\$ (upper)

- **L3.7**

  $\forall f:[a,b]\to\R\textbf{ bounded},$

  $\implies\underline{\int^b_a}f(x)dx\leq\overline{\int^b_a}f(x)dx\\$

- ==**D** Darboux integrable==

  $\forall f:[a,b]\to\R\textbf{ bounded},$

  $\underline{\int^b_a}f(x)dx=\overline{\int^b_a}f(x)dx=:\int^b_af(x)dx\\$

  $\implies f(x)\textbf{ Darboux integrable on }[a,b]$

- **P3.12**

  $\forall f:[a,b]\to\R,$

  $f\textbf{ integrable}\iff\forall\epsilon>0,\exist\text{ partition }P:U(f,P)-L(f,P)<\epsilon$

- **P3.13**

  $\forall(P_n)\text{ partitions of }[a,b],$

  $\lim_{n\to\infin}(U(f,P_n)-L(f,P_n))=0\implies\int^b_af(x)dx=\lim_{n\to\infin}L(f,P_n)=\lim_{n\to\infin}U(f,P_n)\\$

- **T3.16** continuous functions are integrable

  $\forall f:[a,b]\to\R,$

  $f\textbf{ continuous}\implies f\textbf{ integrable}$

- **P6Q2** monotone functions are integrable

  $\forall f:[a,b]\to\R,$

  $f\textbf{ monotonically increasing}\implies f\textbf { integrable}$

- **P3.18**

  $\forall f,g:[a,b]\to\R\textbf{ integrable},$

  $(\forall x\in[a,b],f(x)\leq g(x))\implies\int^b_af(x)dx\leq\int^b_ag(x)dx\\$

- **T3.19** integration is a linear operator

  $\forall f,g:[a,b]\to\R\textbf{ integrable},\forall c,d\in\R,$

  $\int^b_a(cf(x)+dg(x))dx=c\int^b_af(x)dx+d\int^b_ag(x)dx\\$

- **T3.22**

  $\forall f:[a,b]\to\R\textbf{ integrable},\forall c\in(a,b),$

  $\int^b_af(x)dx=\int^c_af(x)dx+\int^b_cf(x)dx\\$

- **T3.23**

  $\forall f:[a,b]\to\R\textbf{ integrable},\text{with }m\leq f(x)\leq M\forall x\in[a,b],$

  $\implies\forall g:[m,M]\to\R\textbf{ continuous},g(f(x))\textbf{ integrable on }[a,b]$

- **P3.24**

  $\forall f:[a,b]\to\R\textbf{ integrable},$

  $\left|\int^b_af(x)dx\right|\leq\int^b_a|f(x)|dx\\$

- **P3.25**

  $\forall f,g:[a,b]\to\R\textbf{ integrable},$

  $f\cdot g:[a,b]\to\R\textbf{ integrable}$

- **P6Q5**

  $\forall f,g:[a,b]\to\R\textbf{ bounded},f$ and $f\cdot g$ both **integrable**,

  $(\forall x\in[a,b],f(x)\geq0\land c\leq g(x)\leq d)\implies$

  $c\int^b_af(x)dx\leq\int^b_af(x)g(x)dx\leq d\int^b_a f(x)dx\\$

- ==**T3.26** fundamental theorem of calculus v1.0==

  $\forall f:[a,b]\to\R\textbf{ continuous},$

  - $F(x):=\int^x_a f(t)dt\\$ **continuous** on $[a,b]$ **differentiable** on $(a,b)$
  - $\forall x\in(a,b),F'(x)=f(x)$

- **T3.27** FTC v2.0

  $\forall f:[a,b]\to\R$ **continuous** with continuous derivative on $(a,b),$

  $\int^b_af'(x)dx=f(b)-f(a)\\$

- **T3.29** Mean value theorem for integrals

  $\forall f:[a,b]\to\R\textbf{ continuous},$

  $\implies\exist c\in(a,b):\int^b_af(x)dx=f(c)(b-a)\\$

- **T3.30** Integration by parts

  $\forall f,g:[a,b]\to\R$ **continuous** with continuous $f',g',$

  $\int^b_af(x)g'(x)dx=f(b)g(b)-f(a)g(a)-\int^b_af'(x)g(x)dx\\$

- **T3.32** Integration by substitution

  $\forall f:[a,b]\to\R\textbf{ continuous},\phi:[c,d]\to[a,b]\text{ with }\phi'\textbf{ continuous on }(c,d),$

  $\int^{\phi(d)}_{\phi(c)}f(x)dx=\int^d_cf(\phi(t))\phi'(t)dt\\$

- **T3.36**

  $\forall f:[a,b]\to\R$ **strictly monotone increasing,**

  $\int^b_af(x)dx+\int^{f(b)}_{f(a)}f^{-1}(x)dx=bf(b)-af(a)\\$

- **T3.40**

  $\forall f_n:[a,b]\to\R$ sequence of **integrable** functions converging uniformly to $f:[a,b]\to\R,$

  $\int^b_af(x)dx=\lim_{n\to\infin}\int^b_af_n(x)dx\\$

- **P3.41** integration of power series

  $\forall f(x):=\sum^\infin_{n=0}a_nx^n\\$ with radius of convergence $R>0,$

  - $f$ **integrable** on any closed subinterval of $(-R,R),$
  - $\forall x\in(-R,R),\int^x_0f(t)dt=\sum^\infin_{n=0}\frac{a_n}{n+1}x^{n+1}\\$

- ==**D** improper integral==

  - $\forall f:(a,b]\to\R$ **integrable** on every subinterval $[c,b]\sub(a,b],$

    $\int^b_af(x)dx=\lim_{c\downarrow a}\int^b_cf(x)dx\\$

  - $\forall f:[a,b)\to\R$ **integrable** on every subinterval $[a,c]\sub[a,b),$

    $\int^b_af(x)dx=\lim_{c\uparrow b}\int^c_af(x)dx\\$

  The improper integral **diverges** if the limit does not exist.

- **P3.48** 

  $\forall f,g:[a,\infin)\to\R,$

  $(\forall x\geq a,0\leq f(x)\leq g(x))\implies$

  - $\exist\int^\infin_ag(x)dx\implies\exist\int^\infin_af(x)dx\\$
  - $0\leq\int^\infin_af(x)dx\leq\int^\infin_ag(x)dx\\$

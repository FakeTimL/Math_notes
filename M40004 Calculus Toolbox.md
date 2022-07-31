## 1. Limits

- **D1** limit

  Let $f:S\rightarrow\R,x_0\in S,l\in\R,$

  $\lim_{x\rightarrow x_0}f(x)=l\iff\\\forall\epsilon>0,\exist\delta>0:\forall x\neq x_0,|x-x_0|<\delta\implies|f(x)-l|<\epsilon$

- **D** properties of limits

  - Assume $\exist\lim_{x\rightarrow x_0}f(x),\lim_{x\rightarrow x_0}g(x),$

    - **(1.1)** Sum rule

      $\lim_{x\rightarrow x_0}[f(x)+g(x)]=\lim_{x\rightarrow x_0}f(x)+\lim_{x\rightarrow x_0}g(x)$
    
    - **(1.2)** Product rule
    
      $\lim_{x\rightarrow x_0}[f(x)g(x)]=\lim_{x\rightarrow x_0}f(x)\lim_{x\rightarrow x_0}g(x)$
  
  - Assume also $\lim_{x\rightarrow x_0}f(x)\neq 0,$
  
    - **(1.3)** Reciprocal rule
  
      $\lim_{x\rightarrow x_0}\left[\frac 1 {f(x)}\right]=\frac 1 {\lim_{x\rightarrow x_0}f(x)}\\$
  
    - **(1.4)** Quotient rule
  
      $\lim_{x\rightarrow x_0}\left[\frac{g(x)}{f(x)}\right]=\frac{\lim_{x\rightarrow x_0}g(x)}{\lim_{x\rightarrow x_0}f(x)}\\$
  
  - Assume also $h(x)$ **continuous** at $\lim_{x\rightarrow x_0}g(x),$
  
    - **(1.5)** Composite function rule
  
      $\lim_{x\rightarrow x_0}[h(g(x))]=h[\lim_{x\rightarrow x_0}g(x)]$


- **D2** limit to infinity $(\epsilon-A)$

  Let $f:(a,\infin)\rightarrow\R,l\in\R,$

  $\lim_{x\rightarrow\infin}f(x)=l\iff\\\forall\epsilon>0,\exist A>a:\forall x>A,|f(x)-l|<\epsilon$

- **D3** limit equals infinity $(\epsilon-B)$

  Let $f:S\rightarrow\R,x_0\in S,$

  $\lim_{x\rightarrow x_0}f(x)=\infin\iff\\\forall B>0,\exist\epsilon>0:\forall x\neq x_0,|x-x_0|<\epsilon\implies f(x)>B$

- **D4** one-sided limit

  Let $f:(x_0,a)\rightarrow\R,l\in\R,$

  $\lim_{x\rightarrow x_0+}f(x)=l\iff\\\forall\epsilon>0,\exist\delta>0:\forall x\in(x_0,x_0+\delta),|f(x)-l|<\epsilon$

- ==**D** squeezing property==

  - $\lim_{x\rightarrow x_0}f(x)=0,|g(x)|\leq|f(x)|\forall x\neq x_0$ (**near**)

    $\implies\lim_{x\rightarrow x_0}g(x)=0$

  - $\lim_{x\rightarrow\infin}f(x)=0,|g(x)|\leq|f(x)|\forall x$ (**large enough**)

    $\implies\lim_{x\rightarrow\infin}g(x)=0$

- **E** trigonometric limits
  - **(1.7)** $\lim_{h\rightarrow 0}\frac{\sin h} h=1\\$
  - **(1.8)** $\lim_{h\to0}\frac{\cos h-1} h=0\\$

- **D5** continuity

  $f$ **continuous** at $x_0$

  - $\iff\lim_{x\rightarrow x_0}f(x)=f(x_0)$
  - $\iff\forall\epsilon>0,\exist\delta>0:\forall x\neq x_0,|x-x_0|<\delta\implies|f(x)-f(x_0)|<\epsilon$



## 2. Differentiation

- **D** differentiability

  $f$ **differentiable** at $x$

  - $\iff\exist f'(x)=\lim_{h\rightarrow0}\frac{f(x+h)-f(x)} h\\$ (**Newton's quotient**)

  - $\iff\exist\lim_{h\rightarrow0+}\frac{f(x+h)-f(x)} h=\lim_{h\rightarrow0-}\frac{f(x+h)-f(x)} h\\$ (**right/left derivatives**)

- **T3** differentiability and continuity

  $f(x)$ **differentiable** at $x=x_0\implies f(x)$ **continuous** at $x=x_0$



## 3. Mean & Intermediate Value

- **D** continuity on interval

  $f$ **continuous** on $[a,b]$

  $\iff\forall x_0\in[a,b],\lim_{x\rightarrow x_0}f(x)=f(x_0)$

- **T2** existence of extrema on interval

  $f$ **continuous** on $[a,b]$

  $\implies\exist c_1,c_2\in[a,b]:\forall x\in[a,b],f(c_1)\leq f(x)\leq f(c_2)$ (**minimum and maximum**)

- **T3** existence of critical point on interval

  Let $f$ **continuous** on $[a,b],$ **differentiable** on $(a,b),$

  $f(a)=f(b)\implies\exist c\in(a,b),f'(c)=0$

- ==**T4** mean value theorem==

  Let $f$ **continuous** on $[a,b],$ **differentiable** on $(a,b),$

  $\implies\exist c\in(a,b),f'(c)=\frac{f(b)-f(a)}{b-a}\\$

- ==**T6** intermediate value theorem==

  $f$ **continuous** on $[a,b]$

  $\implies\forall y\in[f(a),f(b)],\exist x\in[a,b]:f(x)=y$

  

## 4. Inverse Functions

- **D** inverse function

  Let $f:S\rightarrow T,(\forall y\in T,\exist!x\in S:f(x)=y)$

  $\iff\exist f^{-1}:T\rightarrow S,f^{-1}f(x)=x,ff^{-1}(y)=y$

- **T1** increasing/decreasing function has inverse

  $f$ **strictly increasing or decreasing** $\implies\exist f^{-1}$

- **T3** derivative of inverse function

  Let $f$ **differentiable** on $(a,b)$ and **strictly increasing or decreasing**,

  $\implies\exist f^{-1},\frac d {dy}f^{-1}(y)=\frac 1 {f'(x)}\\$

- **E** derivative of trigonometric inverse functions
  - $\frac d {dx}\arcsin(x)=\frac 1 {\sqrt{1-x^2}}\\$
  - $\frac d {dx}\arccos(x)=-\frac 1{\sqrt{1-x^2}}\\$
  - $\frac d{dx}\arctan(x)=\frac 1{1+x^2}\\$



## 5. Exponentials and Logarithms

- **D** natural logarithm

  $\log(x)=\begin{cases}\text{area under }\frac1 x\text{ between 1 and }x&{x>1}\\0&x=1\\-\text{area under }\frac 1 x\text{ between 1 and }x&0<x<1\end{cases}$

- **T1** derivative of $\log$

  $\log$ **differentiable**, $\frac d{dx}\log(x)=\frac 1{x}\\$

- **T3** properties of $\log$

  - $\log$ **strictly increasing**
  - $\log\in(-\infin,\infin)$

- **D** exponential

  - $\exp\log(x)=\log\exp(x)=x$

  - $a^x=\exp(x\log(a))$

- **T6** derivative of $\exp$

  $\exp$ **differentiable**, $\frac d{dx}\exp(x)=\exp(x)\\$

- **T7** derivative of $a^x$

  $\frac d{dx}a^x=a^x\log(a)\\$

- **C** from first principles

  $\forall a>0,\lim_{h\rightarrow 0}\frac{a^h-1} h=\log(a)\\$

- **C1/2** linear and $\log$

  $\lim_{x\rightarrow\infin}(x-\log(x))=\lim_{x\rightarrow\infin}(\frac x{\log(x)})=\infin\\$

- **C3**

  $\lim_{x\rightarrow\infin}(x^{\frac 1x})=1\\$

- **T11** exponential and power

  $\forall m>0,f(x)=\frac{e^x}{x^m}\\$ **strictly increasing** for $x>m,$

  $\lim_{x\rightarrow\infin}f(x)=\infin$

- **T11** L’Hopital’s Rule

  Let $f,g$ **differentiable** on $(a,b),x_0\in(a,b),g'(x_0)\neq 0$

  $g(x_0)=f(x_0)=0\implies\lim_{x\rightarrow x_0}\frac{f(x)}{g(x)}=\frac{f'(x_0)}{g'(x_0)}\\$

- **T12** L'Hopital's Rule converse

  Let $f,g$ **differentiable** on $(a,b),$ **continuous** at $x_0\in(a,b),$ $\forall x\in(a,b)\backslash\{x_0\},g(x)\neq0\land g'(x)\neq 0,$

  $\lim_{x\rightarrow x_0}\frac{f'(x)}{g'(x)}=l\implies\lim_{x\rightarrow x_0}\frac{f(x)}{g(x)}=l\\$

- **T** Cauchy Mean Value Theorem

  Let $f,g$ **continuous** on $[a,b],$ **differentiable** on $(a,b),g(a)\neq g(b)$

  $\implies\exist c\in(a,b):g'(c)\frac{f(b)-f(a)}{g(b)-g(a)}=f'(c)\\$



## 6. Anti-derivatives

- **D** anti-derivative

  $F'(x)=f(x)\iff F(x)$ is the **anti-derivative** of $f(x)$

- **T1** foundamental theorem of calculus

  $\frac d{dx}\int^x_af(t)dt=f(x)\\$

- **D** definite integral

  Let $F(x)$ **differentiable** on $[a,b],F'(x)=f(x),$

  $\int^b_af(x)dx=F(b)-F(a)\\$



## 7. Riemann Sum

- **D** partition

  $f(x)$ can be divided over $[a,b]$ into $n$ **partitions**:

  $\forall 0\leq i\leq n,x_i=a+ih,h=\frac{b-a} n\\$

- **D** Riemann sum

  $\forall0<i\leq n,$ pick $x_i^*\in[x_{i-1},x_i]:$

  - $\sum^n_{i=1}f(x^*_i)h\\$ (**Riemann Sum**)
    - $x^*_i=x_i$ (Upper RS)
    - $x^*_i=x_{i-1}$ (Lower RS)
    - $x^*_i=\frac 1 2(x_i+x_{i-1})$ (Midpoint RS)
  - $\lim_{n\rightarrow\infin,(h\rightarrow 0)}\sum^n_{i=1}f(x^*_i)h=\int^b_af(x)dx\\$



## 8. Properties of the Definite Integral

- **D** title

  - $\forall c\in\R,\int^b_acf(x)dx=c\int^b_af(x)dx\\$
  - $\int^b_a[f(x)+g(x)]dx=\int^b_af(x)dx+\int^b_ag(x)dx\\$
  - $\forall c\in(a,b),\int^b_af(x)dx=\int^c_af(x)dx+\int^b_cf(x)dx\\$

  - $f(x)\leq g(x)\forall x\in[a,b]\implies\int^b_af(x)dx\leq\int^b_ag(x)dx\\$
  - $\int^b_af(x)dx\leq|\int^b_af(x)dx|\leq\int^b_a|f(x)|dx\\$
  - $\int^b_af(x)dx=-\int^a_bf(x)dx\\$

- **T**

  $\frac d{dx}\int^{g(x)}_af(t)dt=f(g(x))\cdot g'(x)\\$



## 10. Improper Integrals

- **D** improper integral

  $\int^b_af(x)dx\\$

  - $a=-\infin$
  - $b=\infin$
  - $\exist x\in(a,b),f(x)\rightarrow\pm\infin$

- **E** find improper integral

  $\int^\infin_af(x)dx=\lim_{b\rightarrow\infin}\int^b_af(x)dx\\$

  **converges** if limit is finite, **diverges** if not

- **E** improper integral of power

  $\int^\infin_1x^rdx\\$ **converges** $\iff r<-1$

- **T** comparison test

  $(\forall x\geq a,|f(x)|\leq g(x))\land(\forall b>a,\exist\int^b_af(x)dx,\int^b_ag(x)dx)\\$

  - $\int^\infin_af(x)dx\\$ **diverges** $\implies\int^\infin_ag(x)dx\\$ **diverges**
  - $\int^\infin_ag(x)dx\\$ **converges** $\implies\int^\infin_af(x)dx\\$ **converges**



## 11. Mean Value Theorem for Integrals

- ==**T** MVT for integrals==

  Let $f$ **continuous** on $[a,b],$

  $\implies\exist x_0\in(a,b):f(x_0)=\frac 1{b-a}\int^b_af(x)dx\\$



## 12. Integration Techniques

- ==**E** trig formulas==
  - $\cos(2x)=2\cos^2(x)-1=1-2\sin^2(x)$
  - $\sin(2x)=2\sin(x)\cos(x)$
  - $\sin(x\pm y)=\sin(x)\cos(y)\pm\cos(x)\sin(y)$
  - $\cos(x\pm y)=\cos(x)\cos(y)\mp\sin(x)\sin(y)$
  - $\sin(x)\cos(y)=\frac 1 2[\sin(x+y)+\sin(x-y)]\\$
  - $\sin(x)\sin(y)=\frac 1 2[\cos(x-y)-\cos(x+y)]\\$
  - $\cos(x)\cos(y)=\frac 1 2[\cos(x+y)+\cos(x-y)]\\$

- **E** trig integrals

  Let $m,n\in\Z,\int\sin^m(x)\cos^n(x)dx:\\$

  - $m=-1,n=1$

    $\int\frac{\cos(x)}{\sin(x)}dx=\log|\sin(x)|+c\\$

  - $n=1$

    $u=\sin(x)\xrightarrow{subs}\int\sin^m(x)\cos(x)dx=\int u^mdu\\$

  - $m,n\neq1$ (reduction formula)

    $=\frac{m-1}{m+n}\int\sin^{m-2}(x)\cos^n(x)dx-\frac{\sin^{m-1}(x)\cos^{n+1}(x)}{m+n}\\$

- **E** trig substitutions

  - $\sqrt{a^2-x^2}$

    $x=a\sin(\theta),dx=a\cos(\theta)d\theta,\sqrt{a^2-x^2}=a\cos(\theta)$

  - $\sqrt{x^2-a^2}$

    $x=a\sec(\theta),dx=a\tan(\theta)sec(\theta)d\theta,\sqrt{x^2-a^2}=a\tan\theta$

  - $\sqrt{a^2+x^2}$ or $a^2+x^2$

    $x=a\tan(\theta),dx=a\sec^2(\theta)d\theta,\sqrt{a^2+x^2}=a\sec(\theta)$

    $x=a\sinh(\theta),dx=a\cosh(\theta)d\theta,\sqrt{a^2+x^2}=a\cosh(\theta)$

- **E** trig recursion

  $I_n=\int\sin^n(x)dx=-\frac1 n\sin^{n-1}(x)\cos(x)+\frac{n-1}nI_{n-2}\\$



## 13. Applications of Integration

- ==**E** length of curves==

  - $L=\int^b_a[1+(f'(x))^2]^{\frac1 2}dx\\$
  - $L=\int^{t_1}_{t_0}\left[(\frac{dx}{dt})^2+(\frac{dy}{dt})^2\right]^{\frac1 2}dt\\$ 	(parametric form)

- **E** volume

  A plane $P$ cuts a solid $V$ at $x\in[a,b]$ with cross-sectional area $A(x)：$

  $V=\int^b_aA(x)dx\\$

- **E** volumes of revolution

  - revolving about the $x$-axis

    $V=\pi\int^b_a(f(x))^2dx\\$

  - revolving about the $y$-axis

    $V=2\pi\int^b_axf(x)dx\\$

- **E** surface areas of revolution

  - revolving about the $x$-axis

    $S=2\pi\int^b_af(x)\sqrt{{1+(f'(x))^2}}dx\\$

  - revolving about the $y$-axis

    $S=2\pi\int^b_ax\sqrt{1+(f'(x))^2}dx\\$

- **E** centres of mass
  - $\textbf{1D}$ - when $n$ masses are placed at $x_i,$
    $\bar x=\frac{\sum^n_{i=1}m_ix_i}{\sum^n_{i=1}m_i}\\$

  - $\textbf{2D}$ - when $n$ masses are placed at $(x_i,y_i),$

    $(\bar x,\bar y)=\frac1{\sum^n_{i=1} m_i}(\sum^n_{i=1} m_ix_i,\sum^n_{i-1} m_iy_i)\\$

  - $\textbf{2D}$ - uniform density of $\{(x,y)|x\in[a,b],y\in[0,f(x)]\}$

    $(\bar x,\bar y)=\frac1{\int^b_af(x)dx}(\int^b_axf(x)dx,\frac 1 2\int^b_a(f(x))^2dx)\\$

  - $\textbf{2D}$ - uniform density of $\{(x,y)|x\in[a,b],y\in[g(x),f(x)]\}$

    $(\bar x,\bar y)=\frac1{\int^b_a(f(x)-g(x))dx}(\int^b_ax(f(x)-g(x))dx,\frac 1 2\int^b_a(f^2(x)-g^2(x))dx)\\$

- **T** Theorem of Pappus

  A region of area $A$ lies on one side of line $l,$ when rotated about $l,$ the **centre of mass** travels distance $d$ and obtains a volume $V:$

  $V=ad$

- **D** moment of inertia

  - A partical of mass $m$ lies at distance $y$ from the $x$-axis, rotates about the $x$-axis with angular velocity $\omega:$
    - **(kinetic energy)** $KE=\frac1 2m(y\omega)^2=\frac1 2\omega^2I\\$
    - **(moment of inertia)** $I=my^2$
  - A collection of masses $m_1\ldots m_n$ lies at distance $y_1\ldots y_n$ from the $x$-axis, rotates with angular velocity $\omega:$
    - **(13.1)** $I=\sum^n_{i=1}m_iy^2_i$
  - A curve $y=f(x)$ with density $\rho(x)$ per unit length has moment of inertia $I_x$ about the $x$-axis and $I_y$ about the $y$-axis:
    - **(13.2)** $I_x=\int^{x_1}_{x_0}\rho(x)f^2(x)\sqrt{1+(f'(x))^2}dx\\$
    - **(13.3)** $I_y=\int^{x_1}_{x_0}\rho(x)x^2\sqrt{1+(f'(x))^2}dx\\$

- **E** length of curves in polar coordinates
  
  A curve $r=f(\theta):$
  
  - $(x,y)=(f(\theta)\cos(\theta),f(\theta)\sin(\theta))$
  - $L=\int^\beta_\alpha\sqrt{(f'(\theta))^2+f^2(\theta)}d\theta=\int^\beta_\alpha\left[(\frac{dr}{d\theta})^2+r^2\right]^\frac1 2d\theta\\$ (from parametric formula)

- **E** area of regions in polar coordinates

  A region bounded by $r=f(\theta)$ within $\theta\in[\alpha,\beta]:$

  $A=\frac1 2\int^\beta_\alpha f^2(\theta)d\theta=\frac1 2\int^\beta_\alpha r^2d\theta\\$



## 14. Further Applications in Physics & Geometry

- **P** change of parameterisation
  $\forall\tau=h(t)$ **monotonic** and **continuous** (its inverse exists),

  $\begin{dcases}x=\phi(t)=x(t)\\y=\psi(t)=y(t)\end{dcases}\xRightarrow{t=\sigma(\tau)}\begin{dcases}x=\phi(\sigma(\tau))=\alpha(\tau)\\y=\psi(\sigma(\tau))=\beta(\tau)\end{dcases}$   	 $(14.5)$

- **D** cycloid

  $\begin{dcases}x=a(t-\sin(t))\\y=a(1-\cos(t))\end{dcases}$                                  	 					 $(14.9)$

- **P** tangent and normal
  
  - $\dot x^2+\dot y^2\neq0\implies$ tangent exists   	 		      	$(14.13)$
  - **tangent:** $(y-y_0)\dot x-(x-x_0)\dot y=0$                   $(14.18)$
  - **normal:** $(y-y_0)\dot y+(x-x_0)\dot x=0$                    $(14.19)$
  
- **P** arc length of rectifiable curves

  - $\frac{dx}{ds}=\frac{\dot{x}}{\sqrt{\dot x^2+\dot y^2}}=\cos\alpha\\$                                     $(14.27)$
  - $\frac{dy}{ds}=\frac{\dot x}{\sqrt{\dot x^2+\dot y^2}}=\sin\alpha\\$                                      $(14.28)$
  - $(\frac{dx}{ds})^2+(\frac{dy}{ds})^2=1\\$                                                $(14.29)$

- **D** curvature

  $\kappa=\frac{d\alpha}{ds}\\$                                                                             $(14.30)$

  - $=\frac{\dot x\ddot y-\ddot x\dot y}{(\dot x^2+\dot y^2)^\frac 3 2}\\$ with parameter $t$                           $(14.33)$

  - $=\frac{dx}{ds}\frac{d^2y}{ds^2}-\frac{dy}{ds}\frac{d^2x}{ds^2}\\$ with parameter $s$
  - $=\frac{y''}{(1+y'^2)^\frac 3 2}\\$ with $y=f(x)$                                  $(14.34)$
  - $>0$ when **convex** and $<0$ when **concave**



## 15. Series

- **D** partial sum

  $\forall\{a_n\}_{n\geq1}\in\R,S_n=\sum^N_{n-1}a_n\\$

- **D** convergence

  $S=\lim_{n\to\infin}\sum^N_{n=1}a_n=\sum^\infin_{n=1}a_n\\$ (series **converges** to sum $S$)

- **T1** series of reciprocals

  $\sum^\infin_{n-1}\frac 1 n\\$ **diverges** $\to+\infin$

- ==**T2** series of power reciprocals==

  $\forall\alpha>1,\sum^\infin_{n=1}\frac 1{n^\alpha}\\$ **converges**

- **T3** necessary condition for convergence

  $\sum^\infin_{n=1}a_n\\$ **converges** $\implies a_n\to0$ as $n\to\infin$

- **D** Cauchy sequence

  $\{S_k\}_{k\geq 1}$ **Cauchy** $\iff$ $\forall\epsilon>0,\exist N\in\N:\forall m,n>N,|S_m-S_n|<\epsilon$

- **C/T4** Cauchy and convergence

  $\{a_n\}$ **Cauchy** $\iff\{a_n\}$ **converges**

- ==**T5** alternating series test==

  $\forall\{a_n\}_{n\geq1}\to0$ *positive and decreasing*

  $\implies\sum^\infin_{n=1}(-1)^{n-1}a_n\\$ **converges**

- ==**T6** comparison test==

  Given $\sum^\infin_{n=1}b_n$ **convergent**, $\{b_n\}\geq 0,b_n\geq|a_n|\forall n$

  $\implies\sum^\infin_{n=1}a_n\\$ **converges**

- **E6** 

  $\forall\alpha>0,|x|<1,\sum^\infin_{n=1}n^\alpha x^n$ **converges**

- **D** absolute and conditional convergence

  $\sum^\infin_{n=1}|a_n|$ **converges** $\implies\sum^\infin_{n=1}a_n$ **absolutely convergent**

  (a series that converges but not absolutely is **conditionally convergent**)

- **T7** absolute convergence

  $\sum^\infin_{n=1}a_n$ **absolutely convergent** $\implies\sum^\infin_{n=1}a_n$ **converges**

- ==**T8** integral test==

  $\forall f(x)$ *positive and decreasing,*

  $\sum^\infin_{n=1}f(n)\\$ **converges** $\iff\int^\infin_1f(x)dx\\$ **converges**

- **E10**

  $\sum^\infin_{n=1}\frac1{n^p}\begin{dcases}\textbf{converges}&p>1\\\textbf{diverges}&\text{otherwise}\end{dcases}$

- ==**T9** ratio test==

  $\lim_{n\to\infin}|\frac{a_{n+1}}{a_n}|=L\implies\sum^\infin_{n=1}a_n\begin{dcases}\textbf{converges absolutely}&L<1\\\textbf{diverges}&L>1\\\text{inconclusive}&\text{otherwise}\end{dcases}\\$

- ==**T10** root test==

  $\lim_{n\to\infin}|a_n|^\frac1 n=L\implies\sum^\infin_{n=1}a_n\begin{dcases}\textbf{converges absolutely}&L<1\\\textbf{diverges}&L>1\\\text{inconclusive}&\text{otherwise}\end{dcases}\\$

- ==**E** general series convergence test==

  $\sum^\infin_{n=1}a_n:\\$

  - if $a_n\to0:$
    - if $\sum^\infin_{n=1}|a_n|$ converges by applying **T2, T6, T8, T9, T10: absolutely convergent**
    - if **T5** applys: **convergent**
    - otherwise: examine the $n^{th}$ Partial sums

  - otherwise: **divergent**



## 16. Power Series

- **D** power series

  $\forall x,\{a_n\}_{n\geq0}\in\R,$

  - $\sum^\infin_{n=0}a_nx^n\\$ (power series)
  - $s_N=\sum^N_{n=0}a_nx^n\\$ (partial sums are degree $N$ polynomials)

- **E** geometric series

  - $\sum^N_{n=0}x^n=\frac{1-x^{N+1}}{1-x}\\$

  - $|x|<1\implies\sum^\infin_{n=0}x^n=\frac1{1-x}\\$ (**converges**)

- **T1** convergence within a range

  $(\exist R>0:\sum^\infin_{n=0}|a_n|R^n\textbf{ converges})\implies\forall|x|<R,\sum^\infin_{n=0}a_nx^n\\$ **converges absolutely**

- ==**D** radius of convergence==

  $\max\{R>0|\sum^\infin_{n=0}|a_n|R^n\textbf{ converges}\}$

  - $\forall|x|<R,\sum^\infin_{n=0}a_nx^n$ **converges absolutely**
  - $x=\pm R$ must be tested separately

- **T2** ratio test for power series

  ==$(\exist\lim_{n\to\infin}\left|\frac{a_{n+1}}{a_n}\right|=L,R=\frac1 L)\implies\\$==

  $\sum^\infin_{n=0}a_nx^n\begin{dcases}\textbf{converges absolutely}&|x|<R\\\textbf{diverges}&|x|>R\\\text{inconclusive}&x=\pm R\end{dcases}$

- ==**T3** root test for power series==

  $\exist\lim_{n\to\infin}|a_n|^\frac1 n=L,R=\frac1 L\\$ (radius of convergence)

- ==**T4/5** calculus with power series==

  Let $f(x)=\sum^\infin_{n=0}a_nx^n,\forall|x|<R,\\$ (*within radius of convergence*)

  - $f'(x)=\sum^\infin_{n=1}na_nx^{n-1}\\$
  - $\int fdx=\sum^\infin_{n=0}\frac{a_nx^{n+1}}{n+1}\\$

- **T6** algebraic operations of power series

  Let $f(x)=\sum^\infin_{n=0}a_nx^n\\$ with radius of convergence $R_1,$

  $g(x)=\sum^\infin_{n=0}b_nx^n\\$ with radius of convergence $R_2,R=\min(R_1,R_2),$

  - $\forall|x|<R,f(x)+g(x)=\sum^\infin_{n=0}(a_n+b_n)x^n\\$
  - $\forall|x|<R,f(x)g(x)=\sum^\infin_{n=0}[\sum^n_{m=0}a_mb_{n-m}]x^n\\$
  - $\forall|x|<R_1,c\neq0,cf(x)=\sum^\infin_{n=0}ca_nx^n\\$



## 17. Taylor Series

- ==**D** Taylor series==

  $f(x)=\sum^\infin_{n=0}a_n(x-x_0)^n=\sum^\infin_{n=0}\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n\\$

  - represents a function $f(x)$ using derivatives at $x=x_0$
  - when $x_0=0,f(x)=\sum^\infin_{n=0}\frac{f^{(n)}(0)}{n!}x^n\\$ (Maclaurin series)

- **E** Taylor expansion of common functions

  - $\sin x=\sum^\infin_{n=0}(-1)^n\frac{x^{2n+1}}{(2n+1)!}\\$
  - $\cos x=\sum^\infin_{n=0}(-1)^n\frac{x^{2n}}{(2n)!}\\$
  - $e^x=\sum^\infin_{n=0}\frac{x^n}{n!}\\$
  - $\ln(1+x)=\sum^\infin_{n=1}(-1)^{n+1}\frac{x^n}{n}\\$

- ==**T1** Taylor's theorem with remainder==

  Assume $f$ has $n+1$ **continuous** derivatives on $[x_0,x]$

  $f(x)=R_n+\sum^n_{i=0}\frac{f^{(i)}(x_0)}{i!}(x-x_0)^i\\$ where $R_n=\int^x_{x_0}\frac{(x-t)^n}{n!}f^{(n+1)}(t)dt\\$

  - $\exist c\in[x_0,x],R_n=f^{(n+1)}(c)\int^x_{x_0}\frac{(x-t)^n}{n!}dt=\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_0)^{n+1}\\$

    as $n\to\infin,R_n\to0\implies$ Taylor series converges to $f(x)$

- **E** alternative Taylor's theorem with $x=x_0+h$

  $f(x_0+h)=R_n(x_0,h)+\sum^n_{i=0}\frac{f^{(i)}(x_0)}{i!}h^i\\$ where

  $R_n=\int^{x_0+h}\frac{(x_0+h-t)^n}{n!}f^{(n+1)}(t)dt\\=\frac{f^{(n+1)}(c)}{(n+1)!}h^{n+1}(\exist c\in[x_0,x_0+h])$

- **E** bounding remainder

  $\exist M_{n+1}\in R,\forall x'\in[x_0,x],|f^{(n+1)}(x')|\leq M_{n+1}\implies$

  $|R_n|\leq M_{n+1}\frac{|x-x_0|^{n+1}}{(n+1)!}\\$

- **D** binomial expansion

  $\forall|x|<1,\alpha\in\R,(1+x)^\alpha=\sum^\infin_{n=0}\frac{\alpha(\alpha-1)\ldots(\alpha-n+1)}{n!}x^n\\$



## 18. Orthogonal & Orthonormal Function Spaces

- **D** inner product

  $\forall f,g:\R\to\R$ Riemann integrable on $[a,b],$

  - $(f,g):=\int^b_a f(x)g(x)dx\\$
  - $(f,f)^\frac1 2:=\|f\|\geq0$

- ==**D** orthogonal and orthonormal system==

  $\forall S=\{\phi_0,\phi_1,\phi_2,\ldots\}\sub\R^\R$ Riemann integrable on $[a,b],$

  - $(\phi_n,\phi_m)=0(\forall m\neq n)\implies S$ **orthogonal** on $[a,b]$
  - Additionally $\|\phi_n\|=1(\forall n)\implies S$ **orthonormal** on $[a,b]$
  - $S'=\{\frac{\phi_n}{\|\phi_n\|}(\forall n)\}\\$ **orthonormal**

- **E** orthonormal trigonometric system

  $S=\{\frac1{\sqrt{2\pi}},\frac{\cos(nx)}{\sqrt\pi},\frac{\sin(nx)}{\sqrt\pi}|n\in\N\}\\$ **orthonormal** on $[a,a+2\pi]\forall a$



## 19. Periodic Functions and Extensions

- **D** periodic functions

  $f(x+T)=f(x)\iff$ $f$ **period** $T\implies$ $f$ **period** $mT(\forall m\in\Z)$

  - $\forall f(x)$ **continuous** on $[a,b]$ can be extended with **period** $T=b-a$

- **D** prescribe values at points of discontinuity

  $\forall\xi,\lim_{x\to\xi_+}f(x)\neq\lim_{x\to\xi_-}f(x)\implies f(\xi)=\frac1 2[f(\xi_+)+f(\xi_-)]\\$

- **E** integral over period

  $\forall f(x)$ **period** $T,$

  - $\forall a,\int^{a+T}_af(x)dx=\int^T_0f(x)dx\\$
  - $\forall\alpha,\beta,\int^\beta_\alpha f(x)dx=\int^{\beta+T}_{\alpha+T}f(x)dx\\$



## 20. Trigonometric Polynomials

- **D** trigonometric polynomial

  $S_n(x)=\frac1 2a_0+\sum^n_{k=1}[a_k\cos(k\omega x)+b_k\sin(k\omega x)]\\$

  - *quasi-periodic* oscillations are obtained if any ratio of the frequencies is irrational

- ==**E** Euler's relation==
  
  - $\cos\theta=\frac1 2(e^{i\theta}+e^{-i\theta})\\$
  - $\sin\theta=\frac1{2i}(e^{i\theta}-e^{-i\theta})=-\frac{i}2(e^{i\theta}-e^{-i\theta})\\$
  
- **E** orthogonality of trigonometric system
  
  - $\int e^{inx}dx=\int(\cos nx+i\sin nx)dx=\frac{e^{inx}}{in}\\$
  - $\int^\pi_{-\pi}e^{inx}dx=\begin{dcases}0&n\neq0\\2\pi&n=0\end{dcases}$

- **E** complex notation for trigonometric polynomials

  - $S_n(x)=\sum^n_{k=-n}\gamma_ke^{ikx}\\$ where

    $\begin{rcases}\gamma_0&=\frac1 2a_0\\\gamma_k&=\frac1 2(a_k-ib_k)\\\gamma_{-k}&=\frac1 2(a_k+ib_k)\end{rcases}\forall1\leq k\leq n$

  - $S_n(x)\in\R\iff\forall1\leq k\leq n,\gamma_k=\gamma^*_{-k}$



## 21. Fourier Series

- ##### **D** Fourier series

  $f(x)=S_N(x)=\frac1 2a_0+\sum^N_{n=1}a_n\cos(nx)+b_n\sin(nx)\\$

- ==**E** Fourier coefficients==

  - $a_n=\frac1\pi\int^\pi_{-\pi}f(x)\cos(nx)dx\\$
  - $b_n=\frac1\pi\int^\pi_{-\pi}f(x)\sin(nx)dx\\$
  
- **E** orthogonality properties

  $\forall m,n\in\Z,$

  - $\int^\pi_{-\pi}\sin(mx)\sin(nx)dx=\int^\pi_{-\pi}\cos(mx)\cos(nx)dx=\begin{dcases}0&m\neq n\\\pi&m=n\neq0\end{dcases}$
  
  - $\int^\pi_{-\pi}\sin(mx)\cos(nx)dx=0\\$
  - $\int^\pi_{-\pi}e^{imx}e^{-inx}dx=\begin{dcases}0&m\neq n\\2\pi&m=n\end{dcases}$

- **T1** Fourier theorem

  $\forall f(x)$ **integrable** on $[-\pi,\pi]$ of bounded variation (has finite number of discontinuities, none of which is infinite),

  ==$f(x)=\frac1 2a_0+\sum^\infin_{n=1}a_n\cos(nx)+b_n\sin(nx)\\$==

  (coefficients defined above) converges to $f(x)$ away from discontinuities, where the value of the function is defined by

  $\frac1 2[f(\xi_+)+f(\xi_-)]\\$

  - $f(x)$ **continuous** $\implies$ convergence **absolute** and **uniform**
  - $f(x)$ **discontinuous** $\implies$ convergence **absolute** and **uniform** everywhere except at discontinuities

- **P** trigonometric identity

  $c_n(x)=\frac1 2+\sum^n_{k=1}\cos(kx)=\frac12\sum^n_{k=-n}e^{ikx}=\frac{\sin((n+\frac1 2)x)}{2\sin(\frac1 2x)}\\$

  - $c_n(2kx):=n+\frac1 2(\forall k\in\Z)\implies c_n$ **continuous** everywhere

- **L1** Riemann-Lebesgue Lemma

  $\forall g(x)$ **integrable** on $[a,b],$

  $I_\lambda=\int^b_ag(x)\sin(\lambda x)dx\xrightarrow{\lambda\to\infin}0\\$

- **L2**

  $\int^\infin_0\frac{\sin(z)}zdz=\frac\pi2\\$

- ==**E** extending to even/odd function on $[-\pi,\pi]$==

  $\forall f(x)\text{ defined on }[0,\pi],n\geq1$

  - even function (only has $\cos$ series)

    - $g(x)=\begin{dcases}f(x)&0\leq x\leq\pi\\f(-x)&-\pi\leq x\leq0\end{dcases}$

    - $a_n=\frac2\pi\int^\pi_0f(x)\cos(nx)dx,b_n=0\\$
    - $g(x)=\frac12a_0+\sum^\infin_{n=1}a_n\cos(nx)\\$

  - odd function (only has $\sin$ series)

    - $g(x)=\begin{dcases}f(x)&0<x<\pi\\-f(-x)&-\pi<x<0\\0&x=0,\pm\pi\end{dcases}$

    - $a_n=0,b_n=\frac2\pi\int^\pi_0f(x)\sin(nx)dx\\$
    - $g(x)=\sum^\infin_{n=1}b_n\sin(nx)\\$

- ==**E** complex form of Fourier series==

  $f(x)=\sum^\infin_{n=-\infin}\gamma_ne^{inx}(\forall|x|\leq\pi)\\$

  $\gamma_n=\frac1{2\pi}\int^\pi_{-\pi}f(x)e^{-inx}dx=\frac12(a_n-ib_n)\\$

  - $\gamma_{-n}=\gamma^*_n=\frac12(a_n+ib_n)\\$
  - $\gamma_0=\frac12a_0\\$

- ###### $2L-$periodic Fourier series

  - **E** orthonormal trigonometric system

    $S=\{\frac1{\sqrt{2L}},\frac{\cos(\frac{n\pi x}L)}{\sqrt L},\frac{\sin(\frac{n\pi x}L)}{\sqrt L}|n\in\N\}\\$ **orthonormal** on $[a,a+2L]\forall a$

  - **E** orthogonality properties

    $\forall m,n\in\Z,$

    - $\int^L_{-L}\sin(\frac{m\pi x}L)\sin(\frac{n\pi x}L)dx=\int^L_{-L}\cos(\frac{m\pi x}L)\cos(\frac{n\pi x}L)dx=\begin{dcases}0&m\neq n\\L&m=n\end{dcases}$
    - $\int^L_{-L}\sin(\frac{m\pi x}L)\cos(\frac{n\pi x}L)dx=0\\$

  - ==**T** Fourier theorem==
    $$
    f(x)=\frac1 2a_0+\sum^\infin_{n=1}a_n\cos(\frac{n\pi x}L)+b_n\sin(\frac{n\pi x}L)
    $$
    where the Fourier coefficients are

    - $a_n=\frac1L\int^L_{-L}f(x)\cos(\frac{n\pi x}L)dx,\qquad n\in\N\\$
    - $b_n=\frac1L\int^L_{-L}f(x)\sin(\frac{n\pi x}L)dx,\qquad n\in\Z^+\\$

  - ==**E** Fourier Theorem, complex form==
    $$
    f(x)=\sum^\infin_{n=-\infin}\gamma_ne^{\frac{in\pi x}L},\qquad|x|<L\\
    $$
    where
    
    - $\gamma_n=\frac1{2L}\int^L_{-L}f(x)e^{-\frac{in\pi x}L}dx,\qquad n\in\Z\\$

- **T** Parseval's theorem

  $f(x)=\frac1 2a_0+\sum^\infin_{n=1}a_n\cos(nx)+b_n\sin(nx)\implies\\$

  $\frac1\pi\int^\pi_{-\pi}f^2dx=\frac12a_0^2+\sum^\infin_{n=1}(a^2_n+b^2_n)\\$

- ==**E** Fourier transform pair==

  $\forall f:\R\to\R,$
  $$
  \hat f(\omega)=\infint f(x)e^{-i\omega x}dx=:\ft{f(x)}\\
  f(x)=\frac1{2\pi}\infint\hat f(\omega)e^{i\omega x}d\omega=:\ift{\hat f(\omega)}
  $$
  

## 1. Fourier Transforms $\newcommand{\ft}[1]{\mathcal F\{#1\}}\newcommand{\ift}[1]{\mathcal F^{-1}\{#1\}}\newcommand{\infint}{\int^\infin_{-\infin}}$

##### - Fourier cosine transform

For $f(x)$ even about $x=0,$
$$
\hat f_c(\omega):=\int^\infin_0f(x)\cos\omega x\,dx=\frac12\hat f(\omega)\\
f(x)=\frac2\pi\int^\infin_0\hat f_c(\omega)\cos\omega x\,d\omega
$$

##### - Fourier sine transform

For $f(x)$ odd about $x=0,$
$$
\hat f_s(\omega):=\int^\infin_0f(x)\sin\omega x\,dx=-\frac1{2i}\hat f(\omega)\\
f(x)=\frac2\pi\int^\infin_0\hat f_s(\omega)\sin\omega x\,d\omega
$$

##### - Transform Properties

- Linearity

$$
\ft{af(x)+bg(x)}=a\hat f(\omega)+b\hat g(\omega)\\
\ift{a\hat f(\omega)+b\hat g(\omega)}=af(x)+bg(x)
$$

- With coefficient $a>0$

$$
\ft{f(ax)}=\frac1a\hat f(\frac\omega a)\\
\ft{f(-x)}=\hat f(-\omega)
$$

- Special case (rectangular pulse)
  $$
  \ft{e^{-a|x|}}=\frac{2a}{a^2+\omega^2}\\
  \ft{f(x):=\begin{dcases}1&|x|\leq a\\0&\text{otherwise}\end{dcases}\;}=\frac2\omega\sin(a\omega)
  $$
  

- Shifted function

$$
\ft{f(x-x_0)}=\hat f(\omega)e^{-i\omega x_0}\\
\ft{f(x)e^{i\omega_0x}}=\hat f(\omega-\omega_0)
$$

- Symmetry formula

$$
\ft{\hat f(x)}=2\pi f(-\omega)
$$

- Differential equations

$$
\ft{\frac{d^nf}{dx^n}}=(i\omega)^n\hat f(\omega)\\
\ft{xf(x)}=i\hat f'(\omega)
$$

- Trigo transforms

$$
\begin{align}
\ft{f'(x)}_c&=-f(0)+\omega\hat f_s(\omega)\\
\ft{f'(x)}_s&=-\omega\hat f_c(\omega)\\
\ft{f''(x)}_c&=-f'(0)-\omega^2\hat f_c(\omega)\\
\ft{f''(x)}_s&=\omega f(0)-\omega^2\hat f_s(\omega)
\end{align}
$$

- Complex conjugate

$$
\ft{[f(x)]^*}=[\hat f(-\omega)]^*
$$

##### - Convolution

$$
f(x)*g(x):=\infint f(x-u)g(u)\,du
$$

###### Convolution theorem

$$
\ft{f*g}=\hat f(\omega)\hat g(\omega)\\
\ft{f(x)g(x)}=\frac1{2\pi}\hat f(\omega)*\hat g(\omega)
$$

###### Energy theorem for $f$ real

$$
\infint[f(x)]^2\,dx=\frac1{2\pi}\infint|\hat f(\omega)|^2\,d\omega
$$

##### - Dirac delta-function

$$
\delta(x)=\lim_{k\to\infin}f_k(x)\\
$$

where $f_k(x)=\begin{dcases}k/2&|x|<1/k\\0&|x|>1/k\end{dcases}$ and that $\infint f_k(x)\,dx=1\\$

###### Sifting property

For $g$ continuous,
$$
\infint g(x)\delta(x-a)\,dx=g(a)
$$

###### Alternative

$$
\delta(x)=\frac1{2\pi}\infint e^{\pm i\omega x}\,d\omega
$$



## 3. Ordinary differential equations

- Ordinary differential equations (ODEs) - concerning one independent variable

  - General form for an ODE of **order** $k$

    $G(x,f(x),\frac{df}{dx},\ldots,\frac{d^kf}{dx^k})=0\\$ (**implicit**)

    - **degree** = power of highest derivative

    - **linear** if $G$ is a linear function of $f(x)$ and its derivatives

    - **explicit** when highest order derivative is a function of lower derivatives

      $\frac{d^kf}{dx^k}=F(x,f(x),\frac{df}{dx},\ldots,\frac{d^{k-1}f}{dx^{k-1}})=0\\$

  - **Solving** ODE = finding $f(x)$ such that the ODE is satisfied over domain of $x$

- **Particular Integral** (or particular solution) is one $f_{PI}(x)$ that satisfy the ODE

  **General solution** is $f_{GS}(x;c_1,c_2,\ldots,c_k)$ with parameters $\{c_i\}^k_{i=1}$ the constants of integration



## 4. First and second order ODEs

### 4.1 First order ODEs

- ==**Separable**==
  - $\frac{dy}{dx}=F_1(y)F_2(x)\\$
  - $\int\frac{dy}{F_1(y)}=\int F_2(x)dx+c_1\\$

- ==**Linear**==
  - $\frac{dy}{dx}+p(x)y=q(x)\\$
  - $y(x)=e^{-\int p(x)dx}\left[\int e^{\int p(x)dx}q(x)dx +c\right]\\$

- **Dimensionally Homogeneous**
  - $\frac{dy}{dx}=F(\frac yx)\\$
  - $y=ux\implies\frac{du}{dx}=\frac{(F(u)-u)}x\\$ (Separable)

- **Bernoulli**
  - $\frac{dy}{dx}+p(x)y=q(x)y^n\\$
  - $y=u^\frac 1{1-n}\implies\frac{du}{dx}+(1-n)p(x)u=(1-n)q(x)\\$ (Linear)



### 4.2 Second order ODEs

- depends on $x$

  - $\frac{d^2y}{dx^2}=F(x)\\$
  - $y_{GS}=\int\left[\int F(x)dx\right]dx+c_1x+c_2\\$

- depends on $x$ and $\frac{dy}{dx}$

  - $\frac{d^2y}{dx^2}=F(x,\frac{dy}{dx})\\$

  - $u=\frac{dy}{dx}\implies\frac{du}{dx}=F(x,u)\\$ (First order)

    $y_{GS}(x)=\int u_{GS}(x;c_1)dx+c_2\\$

- depends on $y$

  - $\frac{d^2y}{dx^2}=F(y)\\$
  - $u=\frac{dy}{dx}\implies\frac{du}{dx}=u\frac{du}{dy}=\frac d{dy}(\frac12 u^2)=F(y)\\$
    - $\frac12u^2=\int F(y)\,dy+c_1=:G(y)+c_1\\$
    - $\frac{dy}{dx}=u=\pm\sqrt{2G(y)+2c_1}\\$ (First order separable)

- depends on $y$ and $\frac{dy}{dx}$ `//TODO`

  - $\frac{d^2y}{dx^2}=F(y,\frac{dy}{dx})\\$
  - $u=\frac{dy}{dx}\implies\frac{du}{dx}=u\frac{du}{dy}=\frac d{dy}(\frac12 u^2)=F(y,u)\\$
    - $\frac{dy}{dx}=u_{GS}(y;c_1)\\$ (First order)

## 5. Linear ODEs

- General form of linear ODE of order $k$

  $$
  \sum^k_{i=0}a_i(x)\frac{d^iy}{dx^i}=f(x)
  $$
  where $a_i(x)$ and $f(x)$ are functions of only independent variable $x$

  - **homogenous** if $f(x)=0,$ inhomogenous otherwise

- Linear Operators

  - $\mathcal D[f]\equiv\frac d{dx}[f]\\$

    Linearity: $\mathcal D^k[\lambda_1f_1+\lambda_2f_2]=\lambda_1\mathcal D^k[f_1]+\lambda_2\mathcal D^k[f_2]$

  - ==$\mathcal L[f]\equiv\sum^k_{i=0}a_i(x)\mathcal D^i[y]\\$==

    Linearity: $\mathcal L[\lambda_1f_1+\lambda_2f_2]=\lambda_1\mathcal L[f_1]+\lambda_2\mathcal L[f_2]$

    - Linear ODE: $\mathcal L[y]=f(x),\mathcal L[y]=0$ (homogenous)
    - Consequence `//TODO`

- Linear independence

  $\left[\sum^k_{i=1}c_if_i(x)=0\iff\{c_i\}^k_{i=1}=0\right]\implies\{f_i(x)\}^k_{i=1}\textbf{ linearly independent}\\$

- ==**P5.1** solution to $\mathcal L[y]=0$== `//TODO`

  $y^H_{GS}(x;c_1,\ldots,c_k)=\sum^k_{i=1}c_iy_i(x)\\$

  where $B=\{y_i(x)\}^k_{i=1}$ is a set of lineary independent solutions

- **P5.2** linear independence test (wronskian matrix)

  $\begin{align}&W[\{y_i(x)\}^k_{i=1}]=\det\mathbb W=\det\left[\begin{matrix}y_1(x)&y_2(x)&\dots&y_k(x)\\\frac{dy_1}{dx}(x)&\frac{dy_2}{dx}(x)&\dots&\frac{dy_k}{dx}(x)\\\vdots&\vdots&&\vdots\\\frac{d^{k-1}y_1}{dx^{k-1}}(x)&\frac{d^{k-1}y_2}{dx^{k-1}}(x)&\dots&\frac{d^{k-1}y_k}{dx^{k-1}}(x)\end{matrix}\right]\neq0\\&\implies\{y_i(x)\}^k_{i=1}\textbf{ linearly independent}\\\end{align}$



### 5.1 General solution of inhomogeneous linear ODE

- Solution to $\mathcal L[y]=f(x)$

  - **complementary function** $y_{CF}$ = solution to $\mathcal L[y]=0$ by **P5.1**
  - **particular integral** $y_{PI}$ = solution to $\mathcal L[y]=f(x)$

  ==$y_{GS}=y_{CF}+y_{PI}$==



### 5.2 First order linear ODEs with constant coefficients

- General form

  $$
  \mathcal L[y]=\sum^k_{i=0}\alpha_i\mathcal D^i[y]=f(x)
  $$

- General form of first order linear ODEs

  $\mathcal L[y]=\alpha_1\frac{dy}{dx}+\alpha_0y=f(x)\\$

  - ==$y_{GS}=c_1e^{-\frac{\alpha_0}{\alpha_1}x}+e^{-\frac{\alpha_0}{\alpha_1}x}\int e^{\frac{\alpha_0}{\alpha_1}x}\frac{f(x)}{\alpha_1}dx\\$==



### 5.3 Second order linear ODEs with constant coefficients

- General form
  $$
  \mathcal L[y]=\alpha_2\frac{d^2y}{dx^2}+\alpha_1\frac{dy}{dx}+\alpha_0y=f(x)
  $$

- ==Characteristic equation==

  $\alpha_2\lambda^2+\alpha_1\lambda+\alpha_0=0$

  - $y_{CF}=y^H_{GS}(x;c_1,c_2)=\begin{dcases}c_1e^{\lambda_1x}+c_2e^{\lambda_2x}&\lambda_1\neq\lambda_2\\c_1e^{\lambda x}+c_2xe^{\lambda x}&\text{repeated root}\end{dcases}$

- Behaviours

  - $a_1^2-4a_0a_2>0\implies\lambda_{1,2}\in\R$

    - $\lambda_1>0$

      $x\to\infin,\quad y_{CF}\to e^{\lambda_1x}\to\infin$

    - $0>\lambda_1>\lambda_2$

      $x\to\infin,\quad y_{CF}\to e^{\lambda_1x}\to0$

  - $a_1^2-4a_0a_2>0\implies\lambda_{1,2}\in\C$

    *See notes P43*

    

### 5.4 k^th^ order Linear ODEs with constant coefficients

- General form
  $$
  \mathcal L[y]=\sum^k_{i=0}a_i\mathcal D^i[y]=f(x)
  $$

- Characteristic equation

  $\sum^k_{i=0}a_i\lambda^i=0\\$

  - All roots are distinct

    $y_{CF}=\sum_{i=1}^kc_ie^{\lambda_ix}\\$

  - Repeated roots

    *See notes P46*



### 5.5 Euler-Cauchy equation

$$
\mathcal L[y]=\sum^k_{i=0}\beta_ix^i\mathcal D^i[y]=f(x)
$$

- Change of variable $x=e^z$

  - $\frac{dy}{dx}=\frac1x\frac{dy}{dz}\\$

  - $\frac{d^2y}{dx^2}=\frac1{x^2}\left[\frac{d^2y}{dz^2}-\frac{dy}{dz}\right]\\$

  - *more details see notes P46*

    

### 5.6 `//TODO`





## 6. Introduction to Systems of ODEs

- General form of system of ODE

  $\begin{dcases}G_1(x,y_1,\ldots,y_n,\frac{dy_1}{dx},\ldots,\frac{dy_n}{dx},\ldots,\frac{d^{k_1}y_1}{dx^{k_1}},\ldots,\frac{d^{k_n}y_n}{dx^{k_n}})=0\\\vdots\\G_n(x,y_1,\ldots,y_n,\frac{dy_1}{dx},\ldots,\frac{dy_n}{dx},\ldots,\frac{d^{k_1}y_1}{dx^{k_1}},\ldots,\frac{d^{k_n}y_n}{dx^{k_n}})=0\end{dcases}$



### 6.1 Systems of first order ODEs

- General form of system of first order ODE

  $\begin{dcases}\frac{dy_1}{dx}=F_1(x,y_1,\ldots,y_n)\\\vdots\\\frac{dy_n}{dx}=F_n(x,y_1,\ldots,y_n)\end{dcases}$

- Turning higher order ODE into system of first order ODEs `//TODO`



### 6.2 Systems of linear first order ODEs with constant coefficients

- General form

  $\begin{dcases}\frac{dy_1}{dx}=\sum^n_{i=1}\alpha_{1i}y_i+g_1(t)\\\vdots\\\frac{dy_n}{dx}=\sum^n_{i=1}\alpha_{ni}y_i+g_n(t)\end{dcases}$

  where $\alpha_{ij}$ are the constant coefficients forming the matrix $A_{n\times n}$

  - matrix form
    $$
    \left[
    	\begin{matrix}
    		\frac{dy_1}{dt}\\
    		\vdots\\
    		\frac{dy_n}{dt}
    	\end{matrix}
    \right]
    =
    \left[
    	\begin{matrix}
    		\alpha_{11}&\dots&\alpha_{1n}\\
    		\vdots&&\vdots\\
    		\alpha_{n1}&\dots&\alpha_{nn}
    	\end{matrix}
    \right]
    \left[
    	\begin{matrix}
    		y_1\\\vdots\\y_n
    	\end{matrix}
    \right]
    +
    \left[
    	\begin{matrix}
    		g_1(t)\\\vdots\\g_n(t)
    	\end{matrix}
    \right]
    $$
    briefly as $\frac{d\vec y}{dt}=A\vec y+\vec g(t)\\$

  - ==linear operator $\mathcal L[\vec y]\equiv(\frac d{dt}-A)\vec y$==

    - System of linear first order ODE: $\mathcal L[\vec y]=\vec g(t)$

    - general solution: $\vec y^H_{GS}=\sum^n_{i=1}c_i\vec y_i\\$ 

      where $c_i$ are arbitrary constants of integration

- ==If $A$ is diagonalisable==

  Diagonalise $A$ to obtain

  $\Lambda:=V^{-1}AV=\text{diag}(\lambda_1,\dots,\lambda_n)$

  where

  $V=\begin{bmatrix}\vec{v_1}&\vec{v_2}&\cdots&\vec{v_n}\end{bmatrix}$

  - **General solution**

    $\vec{y}_{CF}=\sum^n_{i=1}c_ie^{\lambda_it}\vec{v}_i=\text{span}(B:=\{e^{\lambda_1t}\vec{v_1},\dots,e^{\lambda_nt}\vec{v_n}\})\\$

  - **Particular integral**

    Define $\vec u:=V^{-1}\vec y,$

    Solve $\frac{d\vec u}{dt}=\Lambda\vec u+V^{-1}g(t)\\$

    - $\vec y_{PI}=V\vec u$

- If $A$ is not diagonalisable

  With $\vec u:=V^{-1}\vec y$ and **Jordan normal form** $J$ of $A,$

  - **General solution**

    Solve $\frac{d\vec u}{dt}=J\vec u\\$

  - **Particular integral**

    Solve $\frac{d\vec u}{dt}=J\vec u+V^{-1}g(t)\\$

  

##  7. Qualitative analysis of ODEs

### 7.1 Asymptotic behaviour

- Fixed point (equilibrium point)

  $\vec y^*$ is a **fixed point** of a first order ODE system where 
  $$
  \left[\frac{d\vec y}{dt}\right]_{\vec y=\vec y^*}=0
  $$

- Lyapunov stability (around)

  $\forall\epsilon>0,\exist\delta>0:$

  $\lVert\vec y(0)-\vec y^*\rVert<\delta\implies\forall t\geq 0,\lVert\vec y(t)-\vec y^*\rVert<\epsilon$

- Asymptotic stability (converge)

  Lyapunov stable $\land\exist\delta>0:$

  $\lVert\vec y(0)-\vec y^*\rVert<\delta\implies\lim_{t\to\infin}\lVert\vec y(t)-\vec y^*\rVert=0\\$



### 7.2 Phase plane analysis

- A **phase plane** represents the family of solutions to a 2D ODE system starting from different initial conditions
  $$
  \frac{d\vec y}{dt}=A\vec y
  $$

  - A solution $\vec y(t)$ is a **trajectory** of a point moving on the phase plane with **velocity** $\frac{d\vec y}{dt}.\\$ 
  - When the velocities are independent of $t,$ they are **tangent** vectors to the trajectory, forming a **vector field**

- Trajectories in the phase plane cannot cross since initial conditions define *unique* solutions.

  - Exceptions are fixed points and singular points

- **Eigenvectors** of $A$ define lines that are *invariant* (remains on it)

- Phase plane analysis obtains a **phase portrait** of the system

  - Draw lines corresponding to the directions of the eigenvectors and their trajectories
    - Consider asymptotic behaviours as $t\to\infin$
  - Compute vector field at some points and draw representative trajectories
    - [Applet](https://mathlets.org/mathlets/linear-phase-portraits-matrix-entry/)



### 7.3 General system of linear ODEs in 2 dimension

$$
\frac{d\vec y}{dt}=A\vec y;\qquad A=\begin{bmatrix}a&b\\c&d\end{bmatrix}
$$

- The eigenvalues $\lambda$ are obtained by solving
  $$
  \lambda^2-\tau\lambda+\Delta=0
  $$
  where 

  - $\tau=\text{trace}(A):=a+d$
  - $\Delta=\det(A)$

- $\vec y_{GS}=c_1e^{\lambda_1t}\vec v_1+c_2e^{\lambda_2t}\vec v_2$

#### Saddle-point / hyperbolic profile

- $\Delta<0;$ Lower half of $(\tau,\Delta)$
- $\lambda_1\in\R^+,\lambda_2\in\R^-$

- $\vec y(t)\xrightarrow{t\to\infin}c_1e^{\lambda_1}\vec v_1\to\infin$
  - start on $\vec v_2$ direction: $\to0$ 
  - otherwise $\to\infin$ at $\vec v_1$ direction

#### Repelling / unstable node

- $0<\Delta<\frac{\tau^2}4;\tau>0\\$

- $0<\lambda_2<\lambda_1\in\R^+$

- $\vec y(t)\xrightarrow{t\to\infin}c_1e^{\lambda_1}\vec v_1\to\infin$
  - start at $\vec v_2$ direction: $\to\infin$ at $\vec v_2$ direction 
  - otherwise $\to\infin$ at $\vec v_1$ direction

#### Attracting / stable node

- $0<\Delta<\frac{\tau^2}4;\tau<0\\$
- $0>\lambda_1>\lambda_2\in\R^-$
- $\vec y(t)\xrightarrow{t\to\infin}c_1e^{-|\lambda_1|}\vec v_1\to0$
  - start at $\vec v_2$ direction: $\to0$ at $\vec v_2$ direction 
  - otherwise $\to0$ at $\vec v_1$ direction

<u>Other types... (refer to lecture notes)</u>



### 7.5 Extension of phase plane analysis to higher dimensional systems

- $\vec y(t)$ can be considered a trajectory in $\R^n$
- A unique, non-crossing trajectory is defined from each initial condition
- Asymptotic behaviours are considered to draw trajectories
- Vector field: $\frac{d\vec y}{dt}=\vec F(\vec y)\\$
- Fixed points: $\frac{d\vec y}{dt}(\vec y^*)=0\\$

- For general $n$ dimensional linear ODE systems, we have stability if the *real part* of all the eigenvalues are $\in\R^-$



## 8. Introduction to Bifurcations

- **Bifurcations** in an ODE system describe the qualitative change in behaviour by variation of some *parameters* (tunable constants)

### 8.1 Bifurcations in linear systems

- A bifurcation of **linear** systems is defined as a change in stability of the system



### 8.2 Qualitative behaviour of non-linear 1D systems

$$
\frac{dy}{dt}=f(y);\quad y\in\R
$$

- $y(t)$ are trajectories on the real line
- Vector field is the (scalar) velocity as $f(y)\in\R$
- Special points:
  - Fixed points: $f(y^*)=0$
  - Singularities: $f(y_\text{sing})$ undefined



## 9. Partial Differentiation

$$
f:\R^n\to\R
$$

### 9.1 Representation

- Representations for $f:\R^2\to\R$
  - 3D representation with $f(x,y)$ as the height
  - **Contour plot**: level curves $\vec x_C=(x,y)_C$ where $f(\vec x_C)=C$



### 9.2 Limit and continuity

- Limit $\lim_{\vec x\to\vec x^*}f(\vec x)=C\\$

  if $\forall\epsilon>0,\exist\delta>0:$

  $0<|\vec x-\vec x^*|<\delta\implies|f(\vec x)-C|<\epsilon$

- Continuity at $\vec x^*$

  if $\lim_{\vec x\to\vec x^*}f(\vec x)=f(\vec x^*)\\$



### 9.3 Partial differentiation $\newcommand{\diff}[2]{\frac{\partial#1}{\partial#2}}$

- Partial differentiation
  $$
  \diff f{x_i}=\lim_{h\to0}\frac{f(x_1,\ldots,x_i+h,\ldots,x_n)-f(x_1,\ldots,x_n)}h
  $$
  (Partial derivative of $f$ with respect to $x_i$)

  - $\diff{^2f}{y\partial x}=\diff{^2f}{x\partial y}\\$ (Schwarz's theorem)

  

  

### 9.4 Total differentiation

- For $f(x,y)$

  $df=\lim_{\Delta x,\Delta y\to0}\Delta f=(\diff fx)_y\,dx+(\diff fy)_x\,dy\\$

- For $f(x_1,\ldots,x_n)$

  $df=\sum^n_{i=1}(\diff f{x_i})\,dx_i\\$



### 9.5 Chain rule

- For $u(\vec x)$ with $\vec x=\begin{pmatrix}x(t)\\y(t)\end{pmatrix}$

  $\frac{du}{dt}=(\diff ux)_y(\frac{dx}{dt})+(\diff uy)_x(\frac{dy}{dt})\\$

- For $u(\vec x)$ with $\vec x=\begin{pmatrix}\vdots\\x_i(t)\\\vdots\end{pmatrix}$

  $\frac{du}{dt}=\sum^n_{i=1}(\diff u{x_i})\frac{dx_i}{dt}\\$



### 9.6 Implicit functions

- $z=z(x,y)\implies F(x,y,z)=z-z(x,y)=0$
  - $dF=(\diff Fx)_{y,z}\,dx+(\diff Fy)_{x,z}\,dy+(\diff Fz)_{x,y}\,dz=0\\$
  - $dz=(\diff zx)_y\,dx+(\diff zy)_x\,dy\\$

- $(\diff zx)_y=-\frac{(\diff Fx)_{y,z}}{(\diff Fz)_{x,y}}\\$

  $(\diff zy)_x=-\frac{(\diff Fy)_{x,z}}{(\diff Fz)_{x,y}}\\$



### 9.7 Taylor expansion

- $f(x_0+\Delta x)$

  $=f(x_0)+(\frac{df}{dx})_{x_0}\Delta x+\frac12(\frac{d^2f}{dx^2})_{x_0}(\Delta x)^2+\frac1{3!}(\frac{d^3f}{dx3})_{x_0}(\Delta x)^3+\ldots\\$

$\forall f:\R^2\to\R,$

- $f(\vec x_0+\Delta\vec x)$

  $=f(\vec x_0)+\left[(\diff fx)_{\vec x_0}\Delta x+(\diff fy)_{\vec x_0}\Delta y\right]+\\$

  $\frac12\left[(\diff{^2f}{x^2})_{\vec x_0}(\Delta x)^2+2(\diff{^2f}{x\part y})_{\vec x_0}\Delta x\Delta y+(\diff{^2f}{y^2})_{\vec x_0}(\Delta y)^2\right]+\\$

  $\begin{align}\frac1{3!}\left[(\diff{^3f}{x^3})_{\vec x_0}(\Delta x)^3+3(\diff{^3f}{x^2\part y})_{\vec x_0}(\Delta x)^2\Delta y+3(\diff{^3f}{x\part y^2})_{\vec x_0}\Delta x(\Delta y)^2+(\diff{^3f}{y^3})_{\vec x_0}(\Delta y)^3\right]\end{align}$

  $+\ldots$

- Gradient of $f$ at $\vec x_0$

  $\vec\nabla f_{\vec x_0}:=\begin{bmatrix}\diff fx\\\diff fy\end{bmatrix}_{\vec x_0}$

- Hessian matrix associated with $f$ at $\vec x_0$

  $H_{ij}(\vec x_0)=(\diff{^2f}{x_i\part x_j})_{\vec x_0}\\$

- $f(\vec x_0+\Delta\vec x)=f(\vec x_0)+\vec\nabla f(\vec x_0)^T\Delta\vec x+\frac 12\Delta\vec x^TH(\vec x_0)\Delta\vec x+\ldots\\$



## 10 Applications of Multivariate Calculus

### 10.1 Change of Coordinates

- $\vec x=\begin{bmatrix}x\\y\end{bmatrix}=\begin{bmatrix}r\cos\theta\\r\sin\theta\end{bmatrix}$

  $J:=\frac{d\vec x}{d\vec r}=\begin{bmatrix}(\diff xr)_\theta&(\diff x\theta)_r\\(\diff yr)_\theta&(\diff y\theta)_r\end{bmatrix}=\begin{bmatrix}\cos\theta&-r\sin\theta\\\sin\theta&r\cos\theta\end{bmatrix}$

  $d\vec x=J\cdot d\vec r$

- $\vec r=\begin{bmatrix}r\\\theta\end{bmatrix}=\begin{bmatrix}\sqrt{x^2+y^2}\\\arctan\frac yx\end{bmatrix}\\$

  $K:=\frac{d\vec r}{d\vec x}=\begin{bmatrix}(\diff rx)_y&(\diff ry)_x\\(\diff\theta x)_y&(\diff\theta y)_x\end{bmatrix}=\begin{bmatrix}\frac x{\sqrt{x^2+y^2}}&\frac y{\sqrt{x^2+y^2}}\\-\frac y{x^2+y^2}&\frac x{x^2+y^2}\\\end{bmatrix}=\begin{bmatrix}\cos\theta&\sin\theta\\-\frac{\sin\theta}r&\frac{\cos\theta}r\end{bmatrix}$

  $d\vec r=K\cdot d\vec x$

- $J=K^{-1}$

  

### 10.3 Exact ODEs

$$
\frac{dy}{dx}=\frac{-F(x,y)}{G(x,y)}
$$

- Assume solution is of the (implicit) form $u(x,y)=0,$

  $du=(\diff ux)_y\,dx+(\diff uy)_x\,dy=0\\$

  - $\begin{bmatrix}F\\G\end{bmatrix}=\begin{bmatrix}(\diff ux)_y\\(\diff uy)_x\end{bmatrix}$

    $\implies\diff Fy=\diff{^2u}{y\part x}=\diff{^2u}{x\part y}=\diff Gx\\$ (**condition of integrability**)

- if condition holds, `//TODO`

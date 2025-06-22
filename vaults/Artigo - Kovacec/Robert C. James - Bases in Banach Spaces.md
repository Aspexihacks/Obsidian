
# Context

## Shauder Basis

A Shauder Basis for a Banach Space $X$ is a sequence $\{e_{n}\}_{1}^\infty$ of members of $X$ which has the property that for each $x$ in $X$, there is exactly one sequence of scalars $\{x_{i}\}$ for which $x=\sum_{1}^\infty x_{i}e_{i}$ in the sense that $$\lim_{ n \to \infty }\bigg\lvert  \bigg\rvert  x-\sum_{1}^\infty x_{i}e_{i}\bigg\lvert  \bigg\rvert =0.$$
### Orthogonal Sequences in Hilbert Spaces

Any orthogonal sequence in a Hilbert Space $H$ and $x$ is any member of $H$, then there is exactly one sequence $\{x_i\}$ of scalars such that $\lim_{ n \to \infty }\big\lvert  \big\rvert  x-\sum_{1}^\infty x_{i}e_{i}\big\lvert  \big\rvert =0.$ For this sequence of scalars, each $x_{i}$ is $(x,e_{i})$ and$$\bigg\lvert  \bigg\rvert  x-\sum_{1}^\infty x_{i}e_{i}\bigg\lvert  \bigg\rvert=\left[ \sum_{n+1}^\infty \lvert x_{i} \rvert^{2}  \right]^{1/2}.$$
### Some more examples of important Banach Spaces

#### The space $c_{0}$ 

This space is the Banach space of all sequences that are convergent to zero. A basis for this space is $\{e_i\}$ where $e_{i}$ consists of zeros except for 1 position, that position being $i$.
$x \in c_{0} \implies x=(x_{1},x_{2},x_{3},\dots)$ which tells us that the only sequence for which $\lim_{ n \to \infty }\big\lvert  \big\rvert  x-\sum_{1}^\infty x_{i}e_{i}\big\lvert  \big\rvert =0$ is $x$ itself.
For this sequence of scalars $x$, $$\left\lvert  \left\lvert  x-\sum^n_{i=1}x_{i}e_{i} \right\rvert \right\rvert=\max\{\lvert x_{i} \rvert :i>n\}. $$
#### The space $\mathcal{L}_p$ 

An important class of Banach spaces is given by the spaces $\mathcal{L}_p$ for $1 \leqslant p<\infty$, where $\mathcal{L}_p$ is the space of all sequences $x=\left\{x_i\right\}$ for which $\Sigma_1^{\infty}\left|x_i\right|^p$ is convergent and $\|x\|$ is $\left[\Sigma_1^{\infty}\left|x_i\right|^p\right]^{1 / p}$. With $\left\{e_n\right\}$ the same as for $c_0$,

$$
\left\|x-\sum_{i=1}^n x_i e_i\right\|=\left[\sum_{i=n+1}^{\infty}\left|x_i\right|^p\right]^{1 / p} \text { so } \lim _{n \rightarrow \infty}\left\|x-\sum_{i=1}^n x_i e_i\right\|=0 .
$$


# Background

**Definition:** A *Banach Space* is a linear space with either real or complex scalars which has a norm, $\lvert \lvert \cdot \rvert \rvert$, defined in it and is a complete metric space with respect to $d(x,y)=\lvert \lvert x-y \rvert \rvert$.

**Notation:** We will use $lin(A)$ to denote the algebraic linear span of $A$ and $cl[A]$ to denote the closure of $A$.

**Definition:** A Banach space $X$ is said to be *separable* if it contains a dense sequence.
	*Equivalent characterization*: $X$ contains a sequence $\{x_n\}$ for which $X=cl[lin(\{x_{n}\})]$.

**Definition:** A linear mapping $T:X \to Y$ is *continuous* iff it is continuous at 0, or iff there is $\lvert \lvert T \rvert \rvert$ for which$$\sup\{\lvert \lvert Tx \rvert  \rvert:||x||\leq 1 \}=||T||<\infty.\tag{1}$$This number is the least $M$ such that $||Tx||\leq M||x||$ for each $x$.

**Definition:** Two spaces $X,Y$ are said *isomorphic* if there is an algebraic isomorphism $T:X\to Y$ for which both $T$ and $T^{-1}$ are continuous. When this happen, there are $\alpha, \beta>0$ for which $$\alpha||x||\leq||Tx||\leq \beta||x||,\quad x \in X.$$For $\alpha=\beta=1$, $X$ and $Y$ are said *isometric*. 
When $Y$ is just $X$ with some other norm, then the old and new norms are said to be *equivalent* if $X,Y$ are isomorphic with $T=id$.

**Definition:** A *linear functional* is a continuous linear mapping from $X$ into the space of scalars.

**Definition:** The *first dual* of $X$ is the space $X^*$ of all linear functionals on $X$. This space is complete with respect to the norm in $(1)$. 

**Notation:** We usually denote a linear functional $\phi$ with $(\phi,x)$ or $(x,\phi), instead of $\phi(x)$.

**Hahn-Banach Theorem:** If $\phi$ is a linear functional on a linear subset $L$ of a Banach space $X$, then there is a linear functional $\Phi$ on $X$ for which $||\phi||_{L}=||\Phi||$ and $(\Phi,x)=(\phi,x)$ if $x \in L$.
	Sometimes instead of using the theorem it self we might use that for each $x$ nonzero element of $X$ , there is a linear functional $x^{*}$for which $||x^{*}||=1$ and $(x^{*},x)=||x||.$

**Inverse-Mapping Theorem:** If $T$ is a continuous linear one-to-one mapping of a Banach Space $X$ onto a Banach space $Y$, then $T^{-1}$ is continuous.


# The Space $C[0,1]$ 

An example which proves that not all basis can be found as simply as for the spaces talked about before is the space $C[0,1]$. 

## What is the $C[0,1]$ space ?

It is the real space of real-valued functions that are continuous on the closed interval $[0,1]$, with $||f||=\max|f|$ on $[0,1]$. By using this norm, the convergence of a sequence of continuous functions in $C[0,1]$ means uniform convergence.

## How can we describe a basis $\{f_{n}\}$ for $C[0,1]$?

Let $\{t_{i}\}$ be the sequence of dyadic numbers in $[0,1]$: $$0, \frac{1}{2}, \frac{1}{4}, \frac{3}{4}, \frac{1}{8}, \frac{3}{8}, \frac{5}{8}, \frac{7}{8},\dots .$$ 
Now we let $f_{1}=1,f_{2}=t$ and, for each $n>2$, let $$\begin{cases}
f_{n}(t_{j})=0,\quad j<n \\
f_{n}(t_{n})=1
\end{cases}\quad,$$and let $f_{n}$ be linear between any two neighbors among the first $n$ dyadic points.

We now need to show that it is a basis, for this, it will be enough to prove that any $h \in C[0,1]$ has a unique representation as the infinite sum of $a_{i}f_{i},i\geq1$.$$h(0) = a_{1}\cdot 1+ a_{2}\cdot t + 0+0+\dots=a_{1}.$$
$$\begin{align}
h-a_{1}f_{1}=&\sum^\infty_{2}a_{i}f_{i} \land f_{i}(1)=0,i>2 \implies  \\ \implies& a_{2}=h(1)-a_{1}h_{1}(1)=h(1)-a_{1}.
\end{align}$$
 This process can be inductively continued to determine all coefficients uniquely, with 

This process can be inductively continued to determine all coefficients uniquely:$$a_{n}=h(t_{n})-\sum ^{n-1}_{1}a_{i}f_{i}(t_{n}).$$
Since $\{t_i\}$ is dense in $[0,1]$ and $h$ is uniformly continuous, $\sum ^n_{1}a_{i}f_{i}$ converges uniformly to $h$. This basis is also normalized.

# Bases and Projections

If $\{e_{n}\}$ is a basis for $X$, it clearly needs to dense in $X$. *Not being sufficient, even if we suppose the linear independence. An example of this is the sequence of polynomials $\{t^{n-1}:n\geq1\}$ which is not a basis for $C[0,1]$.* 

## A useful inequality

Suppose the linear span of $\{e_n\}$ is dense in $X$, no $e_{n}$ is 0 and there is a positive $K$ such that, for all $n,p \in \mathbb{N}$ and scalars $\{a_{i}\}$,$$K\left\lvert  \left\lvert  \sum^{n+p}_{i=1}  \right\rvert   \right\rvert \geq \left\lvert  \left\lvert  \sum ^{n}_{i=1}a_{i}e_{i}  \right\rvert   \right\rvert. $$
For each $k$, let $x^{*}_{k}$ be a linear functional defined on $lin\{e_{n}\}$ by letting $\left( e^{*}_{k},\sum^{n}_{1}a_{i}e_{i} \right)$ be $a_k$ in $n\geq k$ and 0 otherwise. Then each ${e^*_k}$ is continuous. In fact, for any $x=\sum^{\infty}_{1}x_{i}e_{i}$ with finitely many nonzero terms, $$
\left|\left(e_k^*, x\right)\right|=\left|x_k\right|=\left\|\sum_1^k x_i e_i-\sum_1^{k-1} x_i e_i\right\|/\left\|e_k\right\| \leqslant 2 K\|x\| /\left\|e_k\right\|,$$
so$$\left\|e_k^*\right\| \leqslant \frac{2 K}{\left\|e_k\right\|},$$and $e^{*}_{k}$ can be extended by continuity to all of $X$. 

**Definition:** The linear functionals $\{e^{*}_n\}$ are the *coefficient functionals* of $\{e_{n}\}$.

## An important description of a kind of "independence"

**Theorem:** If the linear span of $\left\{e_n\right\}$ is dense in $X$ and no $e_n$ is 0 , then $\left\{e_n\right\}$ is a basis for $X$ if and only if there is a positive $K$ such that, for all positive integers $n$ and $p$ and scalars $\left\{a_i\right\}$,$$K\left\|\sum_{i=1}^{n+p} a_i e_i\right\| \geqslant\left\|\sum_{i=1}^n a_i e_i\right\| \tag{1}.$$
The least number $K$ satisfying this condition is called *the basis constant* of $\{e_{n}\}$. If the basis constant is 1, $||\sum_{i=1}^n a_i e_i||$ is a monotone increasing function of $n$ and the basis is considered to be *monotone*.

We will usually say that $x$ is *orthogonal* to $y$ if $||x+k||\geq ||x||,\forall k\in \mathbb{R}$.

Any basis $\{e_{n}\}$ becomes monotone if the norm is replaced by the norm $|||\cdot|||$ for which$$|||x|||=\sup\bigg\{\bigg|\bigg|\sum^n_{i=1}\bigg|\bigg|:n\geq 1\bigg\},\quad \text{if }x=\sum^\infty_{i=1}x_{i}e_{i}.$$
This theorem is also described in terms of projections, that is, if we put $\{e_n\}$ as a basis for $X$ and we define $P_{n}(x)$ to be $\sum^n_{1} x_{i}e_{i}$ if $x=\sum^n_{1}x_{i}e_{i}$, then $P_{n}^2=P_{n}$. 

$(1)$ implies $K||x||\geq||P_n(x)||$, so $P_n$ is continuous and $||P_{n}||\leq K$. So, for all $P_n$'s described earlier are projections and their norms are bounded by $K$.

This way, we can now rewrite the theorem in terms of projections:

**Theorem:(Rewritten)** If the linear span of $\left\{e_n\right\}$ is dense in $X$ and no $e_n$ is 0 , then $\left\{e_n\right\}$ is a basis for $X$ if and only if there is a sequence $\{P_{n}\}$ of uniformly bounded projections on $X$ for which the range of $P_n$ is $lin\{e_{i}:i\leq n\}$ and $P_{n}(e_{i})=0$ if $i>n$.
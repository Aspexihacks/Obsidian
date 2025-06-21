
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

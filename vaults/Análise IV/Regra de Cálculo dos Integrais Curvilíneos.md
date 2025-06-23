#Análise 

Seja  $P,Q: D\subseteq \mathbb{R}^2\longrightarrow \mathbb{R}$ onde $\overset{\LARGE \frown}{\small{AB}}$ está em $D$ e é definido pelas equações paramétricas$$\begin{cases}x=\phi(t)\\y=\psi(t)\end{cases}\quad,t\in[t_A,t_B].$$
Consideremos que $\phi,\psi\in C^1[t_A,t_B]$.

Podemos agora considerar 
$$\begin{cases}x_i=\phi(t_i)\\y_i=\psi(t_i)\end{cases}\quad,i=0,1,...,n$$
e pôr $(\xi_i,\eta_i)=(\phi(t_i'),\psi(t_i')),t_i'\in[t_i,t_{i+1}]$.

Tem-se assim, pelo *Teorema do Valor Médio de Lagrange*, que existem $t_i^*,t_i^{**}$ tais que
$$
x_{i+1}-x_i=\phi'(t_i^*)(t_{i+1}-t_i),\ y_{i+1}-y_i=\psi'(t_i^{**})(t_{i+1}-t_i).
$$
Portanto, substituindo, obtemos
$$\begin{aligned}\lim_{\lambda\rightarrow0}&\sum^{n+1}_0P(\xi_i,\eta_i)(x_{i+1}-x_i)+\sum^{n+1}_0Q(\xi_i,\eta_i)(y_{i+1}-y_i)=\\&=\lim_{\lambda\rightarrow0}\sum_0^{n+1}P(\phi(t'_i),\psi(t'_i))\phi'(t''_i)(t_{i+1}-t_i)+Q(\phi(t'_i),\psi(t'_i))\psi'(t'''_i)(t_{i+1}-t_i).\end{aligned}$$
Pela continuidade de $\phi$ e $\psi$, ficamos com
$$\lim_{\lambda\rightarrow0}\sum_0^{n+1}P(\phi(t_i),\psi(t_i))\phi'(t_i)(t_{i+1}-t_i)+Q(\phi(t_i),\psi(t_i))\psi'(t_i)(t_{i+1}-t_i).$$
Ficando com algo do tipo $$\lim_{\lambda\rightarrow0}\sum_0^{n+1}g(t_i)(t_{i+1}-t_i).$$
para $g(t_i)=P(\phi(t_i),\psi(t_i))\phi'(t_i)+Q(\phi(t_i),\psi(t_i))\psi'(t_i)$.

Isto é, $$\begin{aligned}\int_{\overset{\LARGE \frown}{\small{AB}}}P(x,y)\ dx+Q(x,y)\ dy&=\lim_{\lambda\rightarrow 0}\sum^{n-1}_{i=0}P(\xi_i,\eta_i)(x_{i+1}-x_{i})+\sum^{n-1}_{i=0}Q(\xi_i,\eta_i)(y_{i+1}-y_{i})=\\&=\lim_{\lambda\rightarrow0}\sum_0^{n+1}g(t_i)(t_{i+1}-t_i)=\int_{t_A}^{t_B}g(t)\ dt.\end{aligned}$$
Logo, $$\int_{\overset{\LARGE \frown}{\small{AB}}}P(x,y)\ dx+Q(x,y)\ dy= \int_{t_A}^{t_B}P(\phi(t),\psi(t))\phi'(t)+Q(\phi(t),\psi(t))\psi'(t)\ dt.$$

#Análise 

Suponhamos que a força é não constante e que a partícula se move ao longo de um arco de curva $\overset{\LARGE \frown}{\small{AB}}$, retificável, em $\mathbb{R}^2$ de equações 
$$\begin{cases}x=\phi(t)\\y=\psi(t)\end{cases}\quad,t\in[t_A,t_B],$$
com $\phi,\psi\in C^1[t_A,t_B],\phi',\psi'\not=0$.

Neste caso, $F=(P,Q):\overset{\LARGE \frown}{\small{AB}}\rightarrow \mathbb{R}^2$ constitui um campo de forças.

Seja $P=\{t_0=t_A,t_1,...,t_n=t_B\}\subseteq[t_A,t_B]$ partição que divide o arco em subarcos $A_iA_{i+1}$ de comprimento $\Delta S_i,i=0,...,n-1.$

Sendo $t_i^*\in[t_i,t_{i+1}],$ o vetor tangente unitário à curva em $(\phi(t_i^*),\psi(t_i^*))$ é dado por$$\vec{T}(t_i^*)=\frac{(\phi'(t_i^*),\psi'(t_i^*))}{||(\phi'(t_i^*),\psi'(t_i^*))||}.$$
Dado um $\Delta S_i$ suficientemente pequeno, podemos dizer que a partícula se move de forma retilínea com direção e sentido iguais a $\vec{T}(t_i^*)$ e por ação de uma força constante $\vec{F}(\phi(t_i^*),\psi(t_i^*))$.

Desta maneira, o vetor de deslocamento será $||A_iA_{i+1}||\vec{T}(t_i^*)$, sendo o trabalho realizado por $\vec{F},$ ao deslocar a partícula de $A_i$ para $A_{i+1}$, ao longo do arco, é dado por$$\begin{aligned} W_i&\approx(\vec{F}(\phi(t_i^*),\psi(t_i^*))\ |\ ||A_iA_{i+1}||\vec{T}(t_i^*))=\\&=(\vec{F}(\phi(t_i^*),\psi(t_i^*))\ |\ \vec{T}(t_i^*))||A_iA_{i+1}||.\end{aligned}$$

Assim, $$\sum^{n-1}_0(\vec{F}(\phi(t_i^*),\psi(t_i^*))\ |\ \vec{T}(t_i^*))||A_iA_{i+1}||$$
é uma boa aproximação do trabalho ao longo do arco.

Se definirmos o trabalho em si como a redução (em limite) do raio da partição para zero, obtemos que o trabalho é dado pelo integral curvilíneo dxdy do arco.
#Análise

Seja $\overset{\LARGE \frown}{\small{AB}}$ um arco de curva contido em $\mathbb{R}^2$, de equações paramétricas
$$
\begin{cases}x=\phi(t)\\y=\psi(t)\end{cases},t\in[t_A,t_B]
$$
onde $\phi, \psi\in C^1[t_A,t_B],(\phi(t_A),\psi(t_A))=(x_A,y_A)$ e $(\phi(t_B),\psi(t_B))=(x_B,y_B)$ .

Consideremos uma partição $P$ de $[t_A,t_B]$, definida por $\{t_0,t_1,...,t_n\}$ em que
$$
t_A=t_0\leq t_1\leq ...\leq t_n=t_B.
$$
Esta partição induz uma partição $P_1$ em $[x_A,x_B]$, definida por $\{x_0,x_1,...,x_n\}$ e uma partição $P_2$ em  $[y_A,y_B]$, definida por $\{y_0,y_1,...,y_n\}$, tais que
$$
\begin{cases}x_i=\phi(t_i)\\y_i=\psi(t_i)\end{cases}\quad ,i=0,1,...,n.$$
O arco $\overset{\LARGE \frown}{\small{AB}}$ surge , assim, subdividido em arcos $A_iA_{i+1}$ , $i=0,1,...,n-1$, sendo $A=A_0=(x_A,y_A)$ e $B=A_n=(x_B,y_B)$.
Podemos então considerar a linha poligonal, inscrita em $\overset{\LARGE \frown}{\small{AB}}$, ${\LARGE\cup}^{n-1}_{i=0}\overline{A_iA_{i+1}}$.

Representemos então por $C(P)$ o comprimento dessa linha poligonal. Tem-se $C(P)=\sum^{n-1}_{i=0}||\overline{A_iA_{i+1}}||$.
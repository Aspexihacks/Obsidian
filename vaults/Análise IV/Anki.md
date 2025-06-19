TARGET DECK: AI4

Q: ***Proposição*** Uma função $f$ é de *variação limitada* se e só se for possível escrever $f$ como soma algébrica de funções monótonas.
A: $\mathcal{Prova}$ :  Suponhamos que $f$ é de variação limitada. Vamos definir$$\begin{cases}
	f^+(x)= \sup_P\sum^{n-1}_{i=0}max(0,f(x_{i+1})-f(x_i))\\\\
	f^-(x)= \sup_P\sum^{n-1}_{i=0}max(0,f(x_{i})-f(x_{i+1}))
	\end{cases}\quad,$$ onde a soma é tomada em partições de $[a,x], x\in(a,b]$.
	 Como $f^+$ e $f^-$ são monótonas, e é observável que$$f(x)=f(a)+f^+(x)-f^-(x).$$
	 Inversamente, suponhamos que $f$ pode ser escrita como soma de funções monótonas. Então, $f=g_1+g_2+...+g_n$ para funções $g_1,g_2,...,g_n$ monótonas.
	 Como para cada $g_i$ a variação máxima no intervalo de definição (compacto!!) é $|g_i(b)-g_i(a)|$, obtemos que $$\sup_P V(P,f)\leq \sum_1^{n}\sup_PV(P,g_i)\leq\sum_1^{n}|g_i(b)-g_i(a)|<\infty.\square$$
<!--ID: 1749929359522-->

Q: Como medimos um arco de curva? Para evitar a medida de Jordan, que resulta em medida nula.
A: Seja $\overset{\LARGE \frown}{\small{AB}}$ um arco de curva contido em $\mathbb{R}^2$, de equações paramétricas
$$
\begin{cases}x=\phi(t)\\y=\psi(t)\end{cases},t\in[t_A,t_B]
$$
onde $\phi, \psi\in C^1[t_A,t_B],(\phi(t_A),\psi(t_A))=(x_A,y_A)$ e $(\phi(t_B),\psi(t_B))=(x_B,y_B)$ .
<!--ID: 1749930377652-->


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

Q: Qual a definição de variação total de uma função real de variável real?
A: A variação total de $f$ em $[a,b]$ , $V(P,f)$, é dada por$$V(P,f)=\sum^{n-1}_{i=0}|f(t_{i+1})-f(t_i)|.$$
Q: Qual o sentido **positivo** de uma curva $\phi$?
A: Considerando $D$ tal que $fr(D)=\phi$ . Se $D$ se vê à **esquerda** do caminho(/sentido) a ser seguido, esse é o positivo.
<!--ID: 1749930377686-->


Q: Define o integral curvilíneo (dx, dy, dxdy).
A: ![[Pasted image 20250614205300.png]]
<!--ID: 1749930778537-->

Q: Define um campo de vetores conservativo e o seu potencial.
A: ![[Pasted image 20250614205418.png]]
<!--ID: 1749930861962-->


Q: Acha a regra de cálculo dos integrais curvilíneos.
A: ![[Pasted image 20250614205604.png]]![[Pasted image 20250614205612.png]]![[Pasted image 20250614205633.png]]
<!--ID: 1749931011389-->

Q: Podemos estender a definição de integral curvilíneo $dxdy$ a curvas seccionalmente $C^1$.
A: ![[Pasted image 20250614205858.png]]
<!--ID: 1749931363616-->


Q: Prove a seguinte proposição![[Pasted image 20250614210045.png]]
A: ![[Pasted image 20250614210100.png]]
<!--ID: 1749931363639-->


Q: Um integral curvilíneo diz-se **independente da curva** se...
A: ![[Pasted image 20250614210238.png]]
<!--ID: 1749931376307-->

Q: ***Teorema Fundamental do Cálculo para integrais curvilíneos:*** Sejam $\overset{\LARGE \frown}{\small{AB}}$ um arco de curva retificável, de classe $C^1$, e $$F=(P,Q):D\subseteq\mathbb{R^2}\rightarrow\mathbb{R^2}$$onde $\overset{\LARGE \frown}{\small{AB}}\subseteq D$ uma função conservativa e contínua. Então o integral curvilíneo de $F$ em $\overset{\LARGE \frown}{\small{AB}}$ é independente de caminho, sendo $$\int_{\overset{\LARGE \frown}{\small{AB}}}P(x,y)\ dx\ +Q(x,y)\ dy=f(B)-f(A),$$onde $f$ é *função potencial* de $F$.
A: $\mathcal{Prova}:$ Seja $F=\nabla f$, e $\overset{\LARGE \frown}{\small{AB}}$ parametrizado por $$\begin{cases}x=\phi(t)\\y=\psi(t)\end{cases}\quad,\ t\in[t_{A},t_{B}].$$ É fácil ver que $$\begin{align}\int_{\overset{\LARGE \frown}{\small{AB}}}P(x,y)dx+Q(x,y)dy&=\int_{\overset{\LARGE \frown}{\small{AB}}} \frac{\partial f}{\partial x}(x,y) dx +\frac{\partial f}{\partial y}(x,y) dy=\\&= \int_{t_{A}}^{t_{B}} \frac{d}{dt}(f\circ(\phi(t),\psi(t)))dt=\\&=f(\phi(t),\psi(t))\bigg\rvert^{t_{B}}_{t_{A}}=f(B)-f(A).\quad\square\end{align}$$
Q: ***Proposição:*** Sendo $F=(P,Q):D\subseteq \mathbb{R}^2\rightarrow \mathbb{R}^2,$ um campo de vetores contínuo, o integral curvilíneo de $F$ é independente da curva se e só se$$\int_{\gamma}P(x,y)dx+Q(x,y)dy=0,$$para qualquer curva $\gamma$ fechada em $D$.
A: $\mathcal{Prova}:$ Se o integral curvilíneo de $F$ é independente de curva, então dada $\gamma$ uma curva fechada, temos que existe um $C$ tal que $$\begin{align}&\int_{\gamma}P(x,y)dx+Q(x,y)dy=\\&=\int_{\overset{\LARGE \frown}{\small{AC}}}P(x,y)dx+Q(x,y)dy+\int_{\overset{\LARGE \frown}{\small{CA}}}P(x,y)dx+Q(x,y)dy=\\&=\int_{\overset{\LARGE \frown}{\small{AC}}}P(x,y)dx+Q(x,y)dy -\int_{\overset{\LARGE \frown}{\small{AC}}}P(x,y)dx+Q(x,y)dy=0.\end{align}$$Se tivermos que $$\int_{\gamma}P(x,y)dx+Q(x,y)dy=0,$$para qualquer $\gamma$ curva fechada, então temos que dadas duas curvas $\gamma_{1},\gamma_{2}$ que unem $A$ a $B$. Pondo $\gamma=\gamma_{1}\cup(-\gamma_{2})$, temos que  $$\begin{align}&\int_{\gamma}P(x,y)dx+Q(x,y)dy=\\&=\int_{\gamma_{1}}P(x,y)dx+Q(x,y)dy-\int_{\gamma_{2}}P(x,y)dx+Q(x,y)dy=0.\end{align}$$ Logo, $$\int_{\gamma_{1}}P(x,y)dx+Q(x,y)dy=\int_{\gamma_{2}}P(x,y)dx+Q(x,y)dy.$$

**Objetivos**: 
	Consideremos o Teorema Fundamental do Cálculo:
		"Seja $f:[a,b]\rightarrow\mathbb{R}$ contínua, então $\int_a^bf'(x)dx = f(b)-f(a).$"
	 Pretendemos averiguar se é possível generalizar este resultado para $\mathbb{R}^2$, será um integral do tipo $\int\int_D\frac{\partial Q}{\partial y}dxdy$ se poderá relacionar com os valores de $Q$ em $fr(D)$ ou $\int\int_D\frac{\partial P}{\partial x}dxdy$ se poderá relacionar com os valores de $P$ em $fr(D)$.

Para responder a estas questões acabamos por introduzir um novo conceito, o **Integral Curvilíneo**.

Seja $\overset{\LARGE \frown}{\small{AB}}$ um arco de curva contido em $\mathbb{R}^2$ e $f:\overset{\LARGE \frown}{\small{AB}} \rightarrow\mathbb{R}$ uma função contínua.
 Tentemos usar a definição de integral duplo. Considerando $P=\{e_1,e_2,...,e_n\}$ uma partição do arco $\overset{\LARGE \frown}{\small{AB}}$, vem
 $$
 \int\int_{\overset{\LARGE \frown}{\small{AB}}}f(x,y)dxdy=\lim_{\lambda\rightarrow0}\sum^n_{i=1}f(x_i,y_i)mes(e_i)=0.
 $$
Afinal, a **medida de Jordan é nula**. Portanto, o integral de qualquer função contínua definida numa curva seria nulo, tornando isto **MUITO** desinteressante.

Surge então uma necessidade de criar um conceito de medida em $\overset{\LARGE \frown}{\small{AB}}$, diferente do considerado na definição dos integrais anteriores ([[Medidas num arco]]). 


Após sermos capazes de medir, de forma rudimentar, estas curvas podemos começar a ver qual o "limite" desta medida. Para isto, definimos uma **curva retificável**:
		Diz-se que o arco de curva $\overset{\LARGE \frown}{\small{AB}}$  é **retificável** se
		$$
		\sup\{C(P)| P\text{ partição de }[t_A,t_B]\}
		$$
		existir e for finito. Neste caso, este supremo é dito o **comprimento de $\overset{\LARGE \frown}{\small{AB}}$.**

Obtemos, assim, uma nova pergunta à qual queremos responder:
	Como podemos construir um arco de curva retificável?

Tentemos dar resposta...

Sejam $f:[a,b]\rightarrow\mathbb{R}$ e $P$ uma partição de $[a,b]$ por $\{t_0,t_1,...,t_n\}$.

Devemos definir um conceito útil para este tipo de construção:
	A variação total de $f$ em $[a,b]$ , $V(P,f)$, é dada por$$V(P,f)=\sum^{n-1}_{i=0}|f(t_{i+1})-f(t_i)|.$$
    Dizemos que $f$ é de variação limitada se $$\sup_P V(P,f)<\infty.$$
    Isto serve de equivalência à finitude de $V(P,f)$ ao aproximar o diâmetro da partição $P$.

***Proposição*** Uma função $f$ é de *variação limitada* se e só se for possível escrever $f$ como soma algébrica de funções monótonas.
	$\mathcal{Prova}$ :  Suponhamos que $f$ é de variação limitada. Vamos definir$$\begin{cases}
	f^+(x)= \sup_P\sum^{n-1}_{i=0}max(0,f(x_{i+1})-f(x_i))\\\\
	f^-(x)= \sup_P\sum^{n-1}_{i=0}max(0,f(x_{i})-f(x_{i+1}))
	\end{cases}\quad,$$ onde a soma é tomada em partições de $[a,x], x\in(a,b]$.
	 Como $f^+$ e $f^-$ são monótonas, e é observável que$$f(x)=f(a)+f^+(x)-f^-(x).$$
	 Inversamente, suponhamos que $f$ pode ser escrita como soma de funções monótonas. Então, $f=g_1+g_2+...+g_n$ para funções $g_1,g_2,...,g_n$ monótonas.
	 Como para cada $g_i$ a variação máxima no intervalo de definição (compacto!!) é $|g_i(b)-g_i(a)|$, obtemos que $$\sup_P V(P,f)\leq \sum_1^{n}\sup_PV(P,g_i)\leq\sum_1^{n}|g_i(b)-g_i(a)|<\infty.\square$$
***Proposição*** A curva $\overset{\LARGE \frown}{\small{AB}}$ é retificável se e somente se $\phi, \psi$ forem de variação limitada.

Se tivermos um arco retificável, contido em $\mathbb{R}^2$, de equações paramétricas
$$
\begin{cases}x=\phi(t)\\y=\psi(t)\end{cases},t\in[t_A,t_B]
$$
O arco diz-se de **classe $C^1$** se as funções $\phi, \psi$ forem de **classe $C^1$** em $[t_A,t_B]$ e diz-se **simples** se não se intersetar a si próprio, exceto das extremidades.

Definimos agora os seguintes conceitos:
	***Integral Curvilíneo dx:*** Seja $P:D\subseteq \mathbb{R}^2\longrightarrow \mathbb{R}$ , compreendemos como Integral Curvílineo dx o limite $$\lim_{\lambda\rightarrow 0}\sum^{n-1}_{i=0}P(\xi_i,\eta_i)(x_{i+1}-x_{i})\quad(=\int_{\overset{\LARGE \frown}{\small{AB}}}P(x,y)\ dx)$$ se tal existir.
	***Integral Curvilíneo dy:*** Seja $Q:D\subseteq \mathbb{R}^2\longrightarrow \mathbb{R}$ , compreendemos como Integral Curvílineo dy o limite $$\lim_{\lambda\rightarrow 0}\sum^{n-1}_{i=0}Q(\xi_i,\eta_i)(y_{i+1}-y_{i})\quad(=\int_{\overset{\LARGE \frown}{\small{AB}}}Q(x,y)\ dy)$$ se tal existir.
	***Integral Curvilíneo dxdy:*** Seja $P,Q:D\subseteq \mathbb{R}^2\longrightarrow \mathbb{R}$ , compreendemos como Integral Curvílineo dxdy o limite $$\lim_{\lambda\rightarrow 0}\sum^{n-1}_{i=0}P(\xi_i,\eta_i)(x_{i+1}-x_{i})+\sum^{n-1}_{i=0}Q(\xi_i,\eta_i)(y_{i+1}-y_{i})\quad(=\int_{\overset{\LARGE \frown}{\small{AB}}}P(x,y)\ dx+Q(x,y)\ dy)$$ se tal existir.

A [[Regra de Cálculo dos Integrais Curvilíneos]] é bastante simples de se mostrar.

Usando essa mesma regra, podemos provar facilmente que podemos dividir um arco em dois e a soma dos integrais é o integral do arco original.


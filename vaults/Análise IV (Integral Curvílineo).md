
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






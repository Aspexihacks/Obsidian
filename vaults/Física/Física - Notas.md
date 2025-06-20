**Partícula** - Objeto cuja posição pode ser descrita por um único ponto(tudo o que possa ignorar estrutura interna)

**Deslocamento**($SI=metro$) - Grandeza vetorial que nos dá a variação de posição.
	A $dim(\cdot)=1$ o deslocameto pode ser descrito por um escalar:$$\Delta x=x_{f}-x_{i}.$$
	Podemos, na mesma dimensão, descrever a posição e deslocamento por vetores:
	![[Pasted image 20250619132826.png]]

**Velocidade média**($SI=m / s$) - razão entre o deslocamento e intervalo de tempo.

**Rapidez média** - $\frac{\text{distância total percorrida}}{\text{tempo total}}$.

**Velocidade instantânea** - $v(t)=\lim_{ n \to 0 } \frac{{\Delta x}}{\Delta t}=\frac{dx}{dt}$, onde $x(t)$ descreve a posição em função do tempo.

**Aceleração** - taxa de variação da velocidade instantânea.

**Aceleração média** - razão entre a variação de velocidade instantânea e o intervalo de tempo.

**Aceleração instantânea**($SI=\frac{m}{s^2}$) - $a(t)=\lim_{ n \to 0 }\frac{{\Delta v}}{\Delta t}= \frac{dv}{dt}=\frac{d^2x}{dt^2}$.

Usando integração, podemos andar para trás no processo de derivação e passar de aceleração para velocidade, da mesma maneira, podemos passar de velocidade para posição.

Desta maneira, surge a **lei do movimento**:
	$$dx=v\ dt\implies \int^{x(t)}_{x(t_{0})}dx=\int^t_{t_{0}}v(t)dt\implies x(t)=x(t_{0})+\int^t_{t_{0}}v(t)dt$$

de onde a *aceleração média* e a *velocidade média* são dadas por: $$a_m=\frac{{v(t)-v(t_{0})}}{t-t_{0}}=\frac{1}{t-t_{0}}\int^t_{t_{0}}a(t)dt,\quad v_m=\frac{{x(t)-x(t_{0})}}{t-t_{0}}=\frac{1}{t-t_{0}}\int^t_{t_{0}}v(t)dt.$$
Movimentos com aceleração constante são muito comuns na natureza. (*Exemplo:* Queda-livre em proximidades da superfície terrestre.)

Obtemos, com este raciocínio, diversas formas de cálculo para as funções de posição e velocidade:$$a\in \mathbb{R}\text{, constante}$$$$v(t)=v_{0}+\int^t_{t_{0}}a\cdot du=v_{0}+a\cdot(t-t_{0})$$$$x(t)=x_{0}+\int^t_{t_{0}}v\cdot du=x_{0}+v_{0}\cdot(t-t_{0})+\frac{1}{2}\cdot a\cdot(t-t_{0})^2$$
onde $x_0=x(t_{0})$ e $v_0=v(t_{0})$.

Podemos fazer a seguinte transformação:$$\begin{align}
v=v_{0}+a(t-t_{0})&\iff v^2=v_{0}^2+2\cdot v_{0}\cdot a\cdot(t-t_{0})+a^2\cdot(t-t_{0})^2\iff(\text{Subs. por x})\\&\iff v_{0}^2+2\cdot(x-x_{0})
\end{align}$$
Todos os objetos estão sujeitos á mesma aceleração, quando estão nas proximidades da superfície terrestre.

**Gravidade Terrestre:** $g\approx 9,8m/s^2$

**[[Movimento em duas ou três dimensões]]**: Devemos fixar um referencial que seja independente ao movimento e posições.

**Força:** Grandeza vetorial


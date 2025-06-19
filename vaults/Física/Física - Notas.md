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

Desta maneira, surge a *lei do movimento*:
	$dx=v\ dt\implies \int^{x(t)}_{x(t_{0})}dx=\int^t_{t_{0}}v(t)dt\implies x(t)=x(t_{0})+\int^t_{t_{0}}v(t)dt$


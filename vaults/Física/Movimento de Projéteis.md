
Podemos deduzir as formas de cálculo das equações que nos dão as posições dos projéteis em função do tempo.

Assumimos que:
	Aceleração longitudinal é nula ($a_x=0$)
	Aceleração latitudinal é unicamente a aceleração gravítica ($a_y=-g$)
	Pomos $\theta_{0}$ como o ângulo de lançamento
	$v_{0x},v_{0y},x_{0},y_{0}$ correspondes à velocidade inicial de cada coordenada e à posição inicial de cada coordenada

Assim, 
$$v_{0x}=v_{0}\cos \theta_{0},\quad v_{0y}=v_{0}\sin \theta_{0}.$$
Além disso,
$$\begin{cases}
v_{x}=v_{0x}\quad \ \ \ \ \ \ \ \ \quad (a_{x}=0)\\ \\
v_{y}(t)=v_{0y}-gt\quad (a_{y}=-g)
\end{cases}\implies \begin{cases}
x(t)=x_{0}+v_{0x}\cdot t\\ \\
 y(t)=y_{0}+v_{0y}\cdot t - \frac{1}{2}g\cdot t^2
\end{cases}\quad.$$
Como $x=x_{0x}\cdot t \iff \frac{x}{x_{0x}}=t$, temos que $$\begin{align}
y&=v_{0y}\cdot t -\frac{1}{2}g\cdot t=v_{0y}\left( \frac{x}{x_{0x}} \right)-\frac{1}{2}g\left(\frac{x}{x_{0x}}\right)^2=\left( \frac{v_{0y}}{v_{0x}} \right)x-\left( \frac{g}{2v_{0x}^2} \right)x^2=\\&= \frac{\not v_{0}\sin \theta_{0}}{\not v_{0}\cos \theta_{0}}\cdot x -\left( \frac{g}{2\cdot v_{0}^2\cos^2\theta_{0}} \right)x^2=\tan \theta_{0}\cdot x-\left( \frac{g}{2 \cdot v^2_{0}\cos^2\theta_{0}} \right)\cdot x^2
\end{align}$$
Podemos então calcular o *tempo total de voo*, supondo que foi lançado da origem:$$y\left( t_{voo}\right)=v_{0y}t_{voo}-\frac{1}{2}gt_{voo}^{2}=0,t_{voo}>0 \implies t_{voo}=\frac{2v_{0}\sin \theta_{0}}{g}.$$
O *alcance*, com as mesmas suposições, será dado por:$$x(t_{voo})=v_{0x}t_{voo}=v_{0}\cos \theta_{0}\frac{2v_{0}\sin \theta_{0}}{g}=\frac{2v_{0}^{2}}{g}\sin \theta_{0}\cos \theta_{0}=v_{0}^{2} \frac{\sin2\theta_{0}}{g}.$$

#Outros

**Partícula** - Objeto cuja posição pode ser descrita por um único ponto(tudo o que possa ignorar estrutura interna)

**Deslocamento**($SI=metro$) - Grandeza vetorial que nos dá a variação de posição.
	A $dim(\cdot)=1$ o deslocamento pode ser descrito por um escalar:$$\Delta x=x_{f}-x_{i}.$$
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

**Força:** Grandeza vetorial que representa uma interação.

**Interações à distância:** Aquilo que introduz o conceito de *campo*( de forças).

Todas as forças que são observadas na natureza podem ser descritas em função das **quatro interações fundamentais**:
	1. Força Gravitacional
	2. Força Eletromagnética
	3. Força nuclear forte
	4. Força nuclear fraca

As *forças de contacto entre sólidos* encaixam-se em forças eletromagnéticas.

**Força normal:** É a componente de força de contacto *perpendicular* à superfície de contacto.

**Força de atrito:** É a componente de força de contacto *paralela* à superfície de contacto.

Forças de contacto são sempre *distribuídas* ao longo de toda a região de contacto, embora às vezes representemos como forças pontuais.

Os princípios da dinâmica podem ser explicitados pelas ***leis de Newton:*** 
	1. [[Lei da Inércia]]
	2. [[Lei Fundamental da Dinâmica]]
	3. [[Lei da Ação e Reação]]

Uma lei que pode vir a ser útil é a [[Lei da Gravitação Universal]].

Um *diagrama de corpo livre* é uma forma esquemática de apresentar todas as forças que estão a ser aplicadas ou que atuam no sistema em estudo. Podemos seguir alguns passos para criar um destes diagramas:
	1. Identificar o sistema em estudo
	2. Identificar todas as forças que atuam no sistema
	3. Escolher um referencial conveniente
	4. Representar o diagrama usando o referencial as forças e a aceleração
	5. Aplicar a segunda lei de Newton a cada componente de força e aceleração
	6. Tirar conclusões

Exemplo:
![[Pasted image 20250621174101.png]]

Existem algumas [[aplicações para as leis de Newton]] que servem alguns modelos "simples".

**Forças elásticas:** Ocorrem quando esticamos uma mola ou deformamos um corpo sólido e elástico.

Estas forças são-nos dadas pela *Lei de Hooke:*$$\vec{F}=-k\Delta \vec{x}$$onde $k$ é a constante elástica e $\Delta x$ a variação de comprimento da mola (ou sólido) que originou a força.

As forças elásticas têm sempre sentido oposto às deformações que as causam.

O sistema para momentaneamente numa posição de compressão máxima, começando a mover-se no sentido inverso (*a mola tende a voltar ao equilíbrio*). Chegando a essa posição, como o sistema tem velocidade, *não para e começa de novo a distender a mola*. A força restauradora começa a agir em sentido contrário… e *o movimento repete-se indefinidamente* (**oscilações**).

O tipo de movimento descrito acima segue uma onda sinusoidal em função do tempo ($A\cdot\sin\left( \frac{2\pi}{T} t \right)$ ou $A\cdot\cos\left( \frac{2\pi}{T} t \right)$).

**Trabalho:** É realizado por uma força se o ponto de aplicação da mesma se move numa direção não perpendicular à própria força.

**Transferência de Energia:** Dá-se sempre que um sistema realiza trabalho sobre outro.

**Energia Cinética:** Tem haver com o movimento do corpo.

**Energia Potencial:** Está intimamente ligada com a maneira como o sistema está posto.

**Definição:** O *trabalho* é definido como o produto interno da força com o deslocamento do ponto de aplicação.
	Dada uma força constante:$$W=\vec{F}\cdot \Delta \vec{x}=F\Delta x \cos \theta$$onde $F, \Delta x$ são a norma de $\vec{F}, \Delta \vec{x}$ e $\theta$ é o ângulo entre $\vec{F}\text{ e } \Delta \vec{x}$.
	A sua unidade SI é o joule (J).

A nossa questão inicial será então: "Se tivermos uma força não constante, como definimos o trabalho?"

Para definir o trabalho realizado por uma força não constante ao longo de uma distância, devemos representar $F(x)$, uma curva, e fazer partições do domínio, distância a percorrer.

Isto já foi visto em [[Análise IV (Integral Curvílineo)]], dando uma maneira rigorosa de provada de achar o trabalho dada uma força não constante.

O trabalho corresponde então a uma *transferência de energia* para o sistema, isto é, se o trabalho for positivo, então o sistema recebe energia e se o trabalho for negativo, então o sistema perde energia.

**Trabalho total:** Soma algébrica do trabalho que todas as forças realizam sobre um corpo.

**Trabalho da resultante das forças:** Dado um deslocamento $\Delta \vec{r}$ e a força resultante $\vec{F}_{R}=\sum_{i}\vec{F}_{i}$ onde $\vec{F}_{i}$ são forças atuando no corpo, temos como trabalho da resultante das forças$$\vec{F}_{R}\cdot \Delta \vec{r}.$$
A *energia cinética* é por definição dada por $E_{c}\equiv K=\frac{1}{2}mv^{2}(Joule)$.

Há uma importante relação entre a energia cinética e o trabalho:
	**Teorema da Energia Cinética:** O trabalho realizado durante um certo intervalo de tempo pela resultante das forças é igual à variação da sua energia cinética no mesmo intervalo de tempo.
		$\mathcal{Prova:}$ $$\begin{align}
W_{AB}&=\int_{A}^{B}\vec{F}_{res}\cdot d \vec{r} = \int_{A}^{B} F_{res,t}ds=\\&=\int_{A}^{B}ma_{t}ds=\int_{A}^{B}m \frac{dv}{ds}ds=\\&=\int_{A}^{B}mv\ dv=\frac{1}{2}mv^{2}_{B}-\frac{1}{2}mv^{2}_{A}=\Delta K
\end{align}$$
	**Formulação alternativa:** Quando se realiza trabalho sobre um sistema e a única alteração que se observa nesse sistema é a sua velocidade, o trabalho total realizado sobre o sistema é então dado pela variação de energia cinética.

**Potência:** Trabalho realizado por unidade de tempo, sendo a *potência média* dada por $$P_{med}=\frac{W}{\Delta t}.$$
A *potência instantânea (Watt ou J/s)*, tal como a velocidade e aceleração instantânea é dada pela derivada do trabalho, isto é, $$P= \frac{dW}{dt}=\vec{F}\cdot \vec{v}\ \ \ .$$
Em muitos casos, o trabalho realizado por forças externas sobre o sistema não aumenta a energia cinética, mas é armazenado em forma de *energia potencial*.

**Força conservativa:** Força que realiza trabalho nulo sobre um ponto material ao longo de qualquer trajeto fechado. Em [[Análise IV (Integral Curvílineo)]] dizemos que o integral curvilíneo aplicado a essa força é *independente de caminho*.
	Uma característica destas forças é que o trabalho realizado por ela é sempre *reversível*, isto é, toda a energia armazenada como energia potencial pode ser recuperada sem perdas de movimento (em contexto de velocidade/aceleração).

**Forças não conservativas:** São as forças que não são independentes de caminho.
	Algumas destas, como o atrito e resistência num fluido, produzem a dissipação de energia mecânica, estas são chamadas *forças dissipativas*.
	Existem também algumas que produzem um aumento de energia, como explosões, etc.

Para forças conservativas, podemos definir a *função energia potencial* associada a essas forças:$$\Delta \mathcal{U} = \mathcal{U}_{2}-\mathcal{U}_{1}=-\int_{1}^{2}\vec{F}\cdot d \vec{r}.$$
Já vimos [[duas forças de interação que são fontes de  energia potencial]].


**Princípio da conservação da energia:** A energia pode ser convertida de uma forma para a outra ou transmitida de uma região para outra, mas não pode ser criada ou destruída.

Geralmente, a energia total de um sistema é a soma de todas as energias nele, sejam elas mecânicas, térmicas, química, etc. $$E_{sistema}=E_{m}+E_{q}+E_{t}+\dots\ .$$
Se a única fonte de energia transferida for a realização de trabalho sobre o sistema a partir do exterior, então a lei da conservação de energia fica: $$W_{ext}=\Delta E_{sistema}.$$
**Quantidade de movimento:** Grandeza vetorial $\vec{p}$ definida por$$\vec{p}=m \vec{v}.$$
	Também pode ser chamada de *momento linear*.
	Usando esta escrita, vemos a forma original da *segunda lei de Newton*:$$\vec{F}_{res}=\frac{d}{dt}(m \vec{v})=\frac{d \vec{p}}{dt}.$$

O momento **linear** como o nome indica, pode ser tomado como algo **algebricamente linear**, isto é, se $\vec{P}$ for o momento linear de um sistema de $N$ partículas, então com cada partícula tendo momento $\vec{p}_{i},\ i=1,2,\dots,N$, $\vec{P}$ pode se escrito como $$\sum ^{N}_{1} \vec{p}_{i}=\sum^{N}_{1}m_{i} \vec{v}_{i}.$$

Como as forças entre partículas do sistema se anulam duas a duas,$$\sum_{i}\vec{F}_{i}=\sum_{i}\vec{F}_{int,i}+\sum_{i}\vec{F}_{ext,i}=\sum_{i} \vec{F}_{ext,i}=\vec{F}_{ext,res}\quad$$
obtendo então a segunda lei de Newton para um sistema de partículas:$$\vec{F}_{ext,res}=\frac{d \vec{P}}{dt}\iff \begin{cases}
\sum F_{ext,x}=\frac{dP_{x}}{dt} \\
\sum F_{ext,y}=\frac{dP_{y}}{dt} \\
\sum F_{ext,z}=\frac{dP_{z}}{dt}
\end{cases}$$
**Lei da conservação do momento linear:** $$\vec{F}_{ext,res}=0\implies \frac{d \vec{P}}{dt}=0\implies \vec{P}=\sum_{i}m_{i}\vec{v}_{i}=M\vec{v}_{cm}$$onde $M$ é a massa do sistema e $\vec{v}_{cm}$ é a velocidade do centro de massa.
	Mais sobre nestas [[Algumas coisas sobre a Lei da conservação do momento linear|notas]].

Suponhamos que dois corpos entram em contacto durante um intervalo de tempo $\Delta t$. Então, eles exercem forças iguais e opostas um sobre o outro. Ao produto entre a força exercida durante o intervalo de tempo e $\Delta t$, chama-se **Impulso** ($I=F\Delta t$).

Geralmente, como as forças não são constantes, usamos para o cálculo do impulso o valor médio:$$I=\bar{F}\Delta t$$
Isto dá uma "aproximação" retangular (muito mal feita) da área do gráfico da força em aplicação:![[Pasted image 20250624181659.png]]
Logo, vemos que, se quisermos ter o impulso de uma força não constante, devemos usar um integral para achar a área abaixo do gráfico. Isto é, $$\vec{I}=\int^{t_{1}}_{t_{0}}\vec{F}dt$$
O impulso de uma força pode ser usado como uma "medida" do efeito da força. Exemplo:
	É claro que uma explosão de uma bomba faz um efeito mais intenso em milissegundos do que um nadador a empurrar a parede numa partida de costas durante um ou dois segundos.


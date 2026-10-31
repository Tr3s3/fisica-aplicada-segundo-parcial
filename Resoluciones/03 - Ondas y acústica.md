---
tags: [fisica-aplicada, resoluciones, ondas-acustica]
---

# Resoluciones modelo — Ondas y acústica

**Práctica:** [[Ejercicios/03 - Ondas y acústica]] · **Conceptos:** [[Teoría/03 - Conceptos de ondas y acústica]] · **Fórmulas:** [[Teoría/03 - Fórmulas aplicadas de ondas y acústica]]

En cada solución se justifica qué cambia físicamente, se escribe el modelo antes de sustituir y se controla el resultado. Para aprender el planteo, tapa el resto de la solución y avanza un paso a la vez.

---

## 14. Desplazamiento de partículas a partir de presión

![[imagenes/sonido-longitudinal.svg]]

### Interpretación y modelo

Se pide cuánto se desplazan como máximo las partículas de aire. La presión dada es una variación acústica de amplitud, no la presión atmosférica. La onda es sinusoidal y longitudinal, por lo que el cambio de presión está relacionado con la compresión local del medio.

### Datos e incógnitas

$$
\Delta p_{\max}=3.0\times10^{-2}\,\mathrm{Pa},\quad
f=1000\,\mathrm{Hz},\quad
v=344\,\mathrm{m/s},\quad
B=1.42\times10^5\,\mathrm{Pa}.
$$

Se buscan el número de onda $k$ y la amplitud de desplazamiento $s_{\max}$.

### Planteo y cálculo

Primero conectamos frecuencia y longitud de onda mediante $v=\lambda f$. Como $k=2\pi/\lambda$, eliminamos $\lambda$:

$$
k=\frac{2\pi f}{v}
=\frac{2\pi(1000\,\mathrm{s^{-1}})}{344\,\mathrm{m/s}}
=18.27\,\mathrm{rad/m}.
$$

Para una compresión pequeña, $|\Delta p|=B|\Delta V|/V$. En una onda sinusoidal la deformación relativa máxima es $ks_{\max}$; por eso $\Delta p_{\max}=Bks_{\max}$. Despejamos antes de sustituir:

$$
s_{\max}=\frac{\Delta p_{\max}}{Bk}
=\frac{3.0\times10^{-2}\,\mathrm{Pa}}
{(1.42\times10^5\,\mathrm{Pa})(18.27\,\mathrm{m^{-1}})}
=1.16\times10^{-8}\,\mathrm{m}.
$$

### Resultado y control

$$
\boxed{s_{\max}=1.16\times10^{-8}\,\mathrm{m}=11.6\,\mathrm{nm}}
$$

El valor es mucho menor que la longitud de onda $v/f=0.344\,\mathrm{m}$, como corresponde a una onda sonora de pequeña amplitud. La unidad queda en metros porque $\mathrm{Pa}/(\mathrm{Pa/m})=\mathrm{m}$.

> [!warning] No sumar la presión atmosférica
> $3.0\times10^{-2}\,\mathrm{Pa}$ ya es la amplitud de la variación. La presión de equilibrio no se añade al numerador.

---

## 15. Intensidad y nivel sonoro

### Interpretación y modelo

La presión es la amplitud máxima de una onda sinusoidal progresiva. Calculamos primero el flujo de energía por unidad de área; luego expresamos ese flujo en la escala logarítmica de decibeles.

### Datos

$$
\Delta p_{\max}=0.020\,\mathrm{Pa},\quad
\rho=1.20\,\mathrm{kg/m^3},\quad
v=343\,\mathrm{m/s},\quad
I_0=1.0\times10^{-12}\,\mathrm{W/m^2}.
$$

### 1. Intensidad media

Para amplitud máxima de presión:

$$
I=\frac{(\Delta p_{\max})^2}{2\rho v}.
$$

Sustituimos en unidades SI:

$$
I=\frac{(0.020\,\mathrm{Pa})^2}
{2(1.20\,\mathrm{kg/m^3})(343\,\mathrm{m/s})}
=\frac{4.00\times10^{-4}}{823.2}
=4.86\times10^{-7}\,\mathrm{W/m^2}.
$$

### 2. Nivel en decibeles

El nivel compara la intensidad con el umbral de referencia. La razón dentro del logaritmo no tiene unidades:

$$
\beta=10\log_{10}\left(\frac{I}{I_0}\right)
=10\log_{10}\left(
\frac{4.86\times10^{-7}}{1.0\times10^{-12}}
\right)
=10\log_{10}(4.86\times10^5)
=56.9\,\mathrm{dB}.
$$

### Resultado y control

$$
\boxed{I=4.86\times10^{-7}\,\mathrm{W/m^2},\qquad
\beta=56.9\,\mathrm{dB}}
$$

El nivel es positivo porque $I>I_0$. Si se hubiera usado presión eficaz, primero habría que convertirla o usar $I=p_{\mathrm{rms}}^2/(\rho v)$; aquí no se agrega otro factor 2.

---

## 16. Nivel sonoro con una y dos máquinas

### Interpretación y dato del modelo

El modelo indica que cada máquina produce en el puesto del trabajador $2.0\times10^7\,\mathrm{W/m^2}$. Se transcribe el exponente tal como se ve en el escaneo original. Las máquinas son independientes, así que la energía que llega por unidad de tiempo y área se suma.

$$
I_1=2.0\times10^7\,\mathrm{W/m^2},\qquad
I_0=1.0\times10^{-12}\,\mathrm{W/m^2}.
$$

### a) Una máquina

$$
\beta_1=10\log_{10}\left(\frac{I_1}{I_0}\right)
=10\log_{10}\left(\frac{2.0\times10^7}{10^{-12}}\right)
=10\log_{10}(2.0\times10^{19})
=193.0\,\mathrm{dB}.
$$

### b) Dos máquinas iguales

Primero sumamos intensidades, no niveles:

$$
I_{\mathrm{tot}}=I_1+I_1=2I_1
=4.0\times10^7\,\mathrm{W/m^2}.
$$

Después calculamos el nivel total:

$$
\beta_2=10\log_{10}\left(\frac{4.0\times10^7}{10^{-12}}\right)
=10\log_{10}(4.0\times10^{19})
=196.0\,\mathrm{dB}.
$$

La diferencia también puede comprobarse directamente:

$$
\beta_2-\beta_1
=10\log_{10}\left(\frac{2I_1}{I_1}\right)
=10\log_{10}2=3.01\,\mathrm{dB}.
$$

### Resultado y control

$$
\boxed{\beta_1=193.0\,\mathrm{dB},\qquad
\beta_2=196.0\,\mathrm{dB}}
$$

Duplicar la intensidad suma unos $3\,\mathrm{dB}$; no duplica el nivel. El número absoluto es inusualmente alto, pero corresponde al exponente impreso. La conclusión sobre el cambio de $3.01\,\mathrm{dB}$ no depende del valor de $I_1$.

---

## 17. Doppler: fuente que se acerca

![[imagenes/doppler-casos.svg]]

### Interpretación y datos

La ambulancia se mueve hacia un observador quieto respecto del aire. La rapidez del sonido en el medio sigue siendo $340\,\mathrm{m/s}$, pero los frentes emitidos delante de la fuente quedan más juntos.

$$
f_s=500\,\mathrm{Hz},\quad v=340\,\mathrm{m/s},\quad
v_s=+50\,\mathrm{m/s},\quad v_o=0.
$$

El signo de $v_s$ es positivo porque la fuente se acerca al observador.

### Planteo físico

Durante un período de emisión $T_s=1/f_s$, el frente avanza $vT_s$ mientras la ambulancia avanza $v_sT_s$. La separación frontal se reduce a $(v-v_s)T_s$. Entonces:

$$
\lambda'=\frac{v-v_s}{f_s}
=\frac{340-50}{500}
=0.580\,\mathrm{m}.
$$

El observador está quieto y los frentes viajan a $v$, de modo que $f_{\mathrm{obs}}=v/\lambda'$:

$$
f_{\mathrm{obs}}
=\frac{340}{0.580}
=586.2\,\mathrm{Hz}.
$$

Esto equivale a la fórmula general con $v_o=0$:
$$
f_{\mathrm{obs}}=f_s\frac{v}{v-v_s}.
$$

### Resultado y control

$$
\boxed{f_{\mathrm{obs}}\approx586\,\mathrm{Hz}}
$$

La frecuencia aumenta respecto de $500\,\mathrm{Hz}$ porque la fuente se acerca y comprime los frentes que llegan al observador.

---

## 18. Doppler: observador que se aleja

### Interpretación y datos

La sirena está quieta en el aire, por lo que deja frentes con espaciamiento constante. El observador se aleja y se encuentra con ellos más lentamente.

$$
f_s=500\,\mathrm{Hz},\quad v=340\,\mathrm{m/s},\quad
v_s=0,\quad v_o=-30\,\mathrm{m/s}.
$$

$v_o$ es negativo porque nuestra convención toma positivo el movimiento del observador hacia la fuente.

### Planteo físico

Como la fuente está quieta, la longitud de onda en el aire es:

$$
\lambda=\frac{v}{f_s}=\frac{340}{500}=0.680\,\mathrm{m}.
$$

El observador se mueve en sentido contrario a los frentes que lo alcanzan; la rapidez de encuentro es $v-30=310\,\mathrm{m/s}$. Por lo tanto:

$$
f_{\mathrm{obs}}=\frac{310}{0.680}
=455.9\,\mathrm{Hz}.
$$

La fórmula general da lo mismo:
$$
f_{\mathrm{obs}}=f_s\frac{v+v_o}{v-v_s}
=500\frac{340-30}{340-0}.
$$

### Resultado y control

$$
\boxed{f_{\mathrm{obs}}\approx456\,\mathrm{Hz}}
$$

El resultado es menor que la frecuencia emitida, como debe ocurrir cuando el observador se aleja.

---

## 19. Doppler: fuente y observador se acercan

### Interpretación y signos

La fuente avanza hacia el observador y el observador avanza hacia la fuente, ambos respecto del aire:

$$
f_s=500\,\mathrm{Hz},\quad v=340\,\mathrm{m/s},\quad
v_s=+40\,\mathrm{m/s},\quad v_o=+20\,\mathrm{m/s}.
$$

Hay dos efectos diferentes: la fuente reduce el espaciamiento de los frentes y el observador aumenta la rapidez con que los encuentra.

### 1. Espaciamiento producido por la fuente

$$
\lambda'=\frac{v-v_s}{f_s}
=\frac{340-40}{500}
=0.600\,\mathrm{m}.
$$

### 2. Frecuencia de encuentro del observador

Los frentes se acercan al observador a rapidez relativa $v+v_o=340+20=360\,\mathrm{m/s}$:

$$
f_{\mathrm{obs}}=\frac{v+v_o}{\lambda'}
=\frac{360}{0.600}
=600\,\mathrm{Hz}.
$$

También:
$$
f_{\mathrm{obs}}=f_s\frac{v+v_o}{v-v_s}
=500\frac{340+20}{340-40}.
$$

### Resultado y control

$$
\boxed{f_{\mathrm{obs}}=600\,\mathrm{Hz}}
$$

Los dos movimientos son de acercamiento, así que ambos contribuyen a elevar la frecuencia. El resultado supera tanto la frecuencia emitida como el caso de un solo objeto en movimiento.

---

## 20. Rapidez del sonido y longitudes de onda en distintos medios

### a) Sonido en agua

El medio es un fluido y se conocen su módulo volumétrico y densidad. La rapidez sale del equilibrio entre elasticidad e inercia:

$$
v=\sqrt{\frac{B}{\rho}}
=\sqrt{\frac{2.20\times10^9\,\mathrm{Pa}}
{1.00\times10^3\,\mathrm{kg/m^3}}}
=1.483\times10^3\,\mathrm{m/s}.
$$

La longitud de onda se obtiene con la frecuencia de la fuente y la rapidez del medio:

$$
\lambda=\frac{v}{f}
=\frac{1483\,\mathrm{m/s}}{262\,\mathrm{s^{-1}}}
=5.66\,\mathrm m.
$$

**Resultado:** $v_{\mathrm{agua}}\approx1483\,\mathrm{m/s}$ y $\lambda\approx5.66\,\mathrm m$. La frecuencia no se multiplica por una rapidez nueva; el cociente $v/f$ da una longitud.

### b) Onda longitudinal en plomo

Una varilla delgada transmite una deformación longitudinal, por eso se usa el módulo de Young $Y$:

$$
v\approx\sqrt{\frac{Y}{\rho}}
=\sqrt{\frac{1.60\times10^{10}\,\mathrm{Pa}}
{1.13\times10^4\,\mathrm{kg/m^3}}}
=1.190\times10^3\,\mathrm{m/s}.
$$

**Resultado:** $v_{\mathrm{plomo}}\approx1190\,\mathrm{m/s}$. Se usa la densidad y elasticidad del plomo, no las propiedades del aire.

### c) Sonido en aire y rango audible

Convertimos la temperatura antes de usar la relación del gas ideal:

$$
T=20+273.15=293.15\,\mathrm K.
$$

Entonces:

$$
v=\sqrt{\frac{\gamma RT}{M}}
=\sqrt{\frac{(1.40)(8.314\,\mathrm{J/(mol\,K)})(293.15\,\mathrm K)}
{28.8\times10^{-3}\,\mathrm{kg/mol}}}
=344.2\,\mathrm{m/s}.
$$

La longitud de onda es mayor para la frecuencia menor:

$$
\lambda_{20}=\frac{344.2}{20}=17.2\,\mathrm m,\qquad
\lambda_{20\,000}=\frac{344.2}{20\,000}=1.72\times10^{-2}\,\mathrm m.
$$

**Control:** el sonido audible va, aproximadamente, desde ondas de unos $17\,\mathrm m$ a $1.7\,\mathrm{cm}$ en este modelo. La temperatura se introdujo en kelvin.

---

## 21. Igual intensidad con dos frecuencias

### Modelo e incógnitas

Ambas ondas viajan en el mismo aire, así que $\rho$ y $v$ no cambian. Para una onda progresiva sinusoidal usamos:

$$
I=\frac{\Delta p_{\max}^2}{2\rho v}.
$$

### 1) Intensidad de la onda de $1000\,\mathrm{Hz}$

$$
I=\frac{(3.0\times10^{-2}\,\mathrm{Pa})^2}
{2(1.20\,\mathrm{kg/m^3})(344\,\mathrm{m/s})}
=1.09\times10^{-6}\,\mathrm{W/m^2}.
$$

### 2) Amplitud de presión de la onda de $20\,\mathrm{Hz}$

Con el mismo medio, igual intensidad exige igual amplitud máxima de presión porque la fórmula depende de $\Delta p_{\max}^2$:

$$
\Delta p_{2,\max}=\Delta p_{1,\max}=3.0\times10^{-2}\,\mathrm{Pa}.
$$

### 3) Desplazamientos

Usamos la forma $\Delta p_{\max}=\rho v\omega s_{\max}$, despejada para $s_{\max}$:

$$
s_{\max}=\frac{\Delta p_{\max}}{\rho v\,2\pi f}.
$$

Para $1000\,\mathrm{Hz}$:

$$
s_{1000}=
\frac{0.030}{(1.20)(344)(2\pi)(1000)}
=1.16\times10^{-8}\,\mathrm m.
$$

Para $20\,\mathrm{Hz}$:

$$
s_{20}=
\frac{0.030}{(1.20)(344)(2\pi)(20)}
=5.78\times10^{-7}\,\mathrm m.
$$

**Resultado y lectura física:**

$$
\boxed{I=1.09\times10^{-6}\,\mathrm{W/m^2},\quad
\Delta p_{2,\max}=0.030\,\mathrm{Pa},\quad
s_{20}=50\,s_{1000}.}
$$

La frecuencia de $20\,\mathrm{Hz}$ es cincuenta veces menor; para conservar igual intensidad y presión máxima, la amplitud de movimiento debe ser cincuenta veces mayor.

---

## 22. Transmisión de presión al fluido del oído

### Interpretación del modelo

La presión del aire ejerce una fuerza sobre el tímpano. El TP idealiza la transmisión suponiendo que esa fuerza llega al estribo, cuya área es menor. Como $F=pA$, el mismo empuje sobre menor área produce mayor presión.

### 1) Presión en el fluido del oído

Las áreas están ambas en $\mathrm{mm^2}$, así que el cociente no requiere conversión:

$$
\Delta p_{f,\max}A_e
=\Delta p_{\mathrm{aire},\max}A_t,
\qquad
\Delta p_{f,\max}
=\Delta p_{\mathrm{aire},\max}\frac{A_t}{A_e}.
$$

$$
\Delta p_{f,\max}
=(3.0\times10^{-2})\frac{43}{3.2}
=0.403\,\mathrm{Pa}.
$$

### 2) Desplazamiento en el fluido

La frecuencia se mantiene al transmitirse la vibración. Para el fluido del oído:

$$
s_{f,\max}
=\frac{\Delta p_{f,\max}}{\rho_f v_f\,2\pi f}
=\frac{0.403}{(1.00\times10^3)(1500)(2\pi)(1000)}
=4.28\times10^{-11}\,\mathrm m.
$$

**Resultado:**

$$
\boxed{\Delta p_{f,\max}\approx0.403\,\mathrm{Pa},\qquad
s_{f,\max}\approx4.28\times10^{-11}\,\mathrm m.}
$$

La densidad usada es la aproximación al agua indicada en el ejercicio redactado. No se reutiliza la densidad del aire dentro de la relación de desplazamiento del fluido.

---

## 23. Potencia acústica y cambio con la distancia

### 1) Potencia de la fuente

La hipótesis dice que la fuente irradia por igual en todas direcciones. A $20\,\mathrm m$, su potencia cruza una esfera de área $4\pi r_1^2$:

$$
P_{\mathrm{ac}}=4\pi r_1^2 I_1
=4\pi(20\,\mathrm m)^2(1.0\,\mathrm{W/m^2})
=5.03\times10^3\,\mathrm W.
$$

### 2) Intensidad a $40\,\mathrm m$

La misma potencia ahora se distribuye sobre una esfera cuatro veces mayor:

$$
I_2=\frac{P_{\mathrm{ac}}}{4\pi r_2^2}
=\frac{5.03\times10^3}{4\pi(40)^2}
=0.250\,\mathrm{W/m^2}.
$$

También se ve directamente con la ley del inverso del cuadrado:

$$
\frac{I_2}{I_1}=\left(\frac{r_1}{r_2}\right)^2
=\left(\frac{20}{40}\right)^2=\frac14.
$$

### 3) Cambio de nivel

No necesitamos calcular los dos niveles absolutos: al restarlos, la intensidad de referencia se cancela.

$$
\Delta\beta=10\log_{10}\left(\frac{I_2}{I_1}\right)
=10\log_{10}(0.25)
=-6.02\,\mathrm{dB}.
$$

### 4) Intensidad a partir de un nivel en decibeles

Despejamos la definición del nivel:

$$
\beta=10\log_{10}\left(\frac I{I_0}\right)
\quad\Longrightarrow\quad
I=I_0\,10^{\beta/10}.
$$

Para $28\,\mathrm{dB}$:

$$
I_{28}=10^{-12}\,10^{28/10}
=10^{-12}\,10^{2.8}
=6.31\times10^{-10}\,\mathrm{W/m^2}.
$$

Para $92\,\mathrm{dB}$:

$$
I_{92}=10^{-12}\,10^{92/10}
=10^{-12}\,10^{9.2}
=1.58\times10^{-3}\,\mathrm{W/m^2}.
$$

**Resultado:** se requieren unos $5.03\,\mathrm{kW}$ en el modelo isotrópico; a doble distancia la intensidad queda en un cuarto y el nivel baja $6.02\,\mathrm{dB}$. La inversión del logaritmo muestra que $92\,\mathrm{dB}$ corresponde a una intensidad mucho mayor que $28\,\mathrm{dB}$.

---

## 24. Interferencia de dos altavoces coherentes

### 1) Diferencia de caminos

Las dos fuentes llegan al mismo punto por trayectos de $5.00\,\mathrm m$ y $4.00\,\mathrm m$:

$$
\Delta r=|r_A-r_B|=|5.00-4.00|=1.00\,\mathrm m.
$$

Como emiten en fase, la diferencia de camino determina directamente el desfase.

### 2) Frecuencias constructivas

Para un máximo, $\Delta r=m\lambda$, con entero positivo $m$. Sustituimos $\lambda=v/f$ y despejamos:

$$
f_m=\frac{mv}{\Delta r}
=\frac{m(350\,\mathrm{m/s})}{1.00\,\mathrm m}.
$$

Para $m=1,2,3$:

$$
f=350,\ 700,\ 1050\,\mathrm{Hz}.
$$

$m=0$ daría frecuencia nula, por eso no forma parte de las frecuencias sonoras positivas pedidas.

### 3) Frecuencias destructivas

Para un mínimo, $\Delta r=(m+\tfrac12)\lambda$:

$$
f_m=\frac{(m+\tfrac12)v}{\Delta r}.
$$

Con $m=0,1,2$:

$$
f=175,\ 525,\ 875\,\mathrm{Hz}.
$$

**Control:** los mínimos quedan a medio camino entre máximos sucesivos. Si las fuentes no fueran coherentes o no emitieran en fase, estas condiciones necesitarían incorporar su diferencia de fase inicial.

---

## 25. Cancelación del sonido reflejado por una pared

Primero calculamos la longitud de onda en aire:

$$
\lambda=\frac{v}{f}
=\frac{340\,\mathrm{m/s}}{680\,\mathrm{s^{-1}}}
=0.500\,\mathrm m.
$$

En una pared rígida ideal, la presión incidente y reflejada se suman en la superficie. Al alejarnos, los primeros nodos de presión aparecen a distancias impares de un cuarto de longitud de onda:

$$
x_n=\frac{(2n+1)\lambda}{4},\qquad n=0,1,2,\ldots
$$

Para los tres primeros:

$$
x_0=\frac{0.500}{4}=0.125\,\mathrm m,
\quad
x_1=\frac{3(0.500)}4=0.375\,\mathrm m,
\quad
x_2=\frac{5(0.500)}4=0.625\,\mathrm m.
$$

**Resultado:** los nodos ideales están a $0.125$, $0.375$ y $0.625\,\mathrm m$ de la pared. En una habitación real, otras reflexiones y la absorción impiden que esos puntos sean silencios perfectos.

---

## 26. Longitudes de onda delante y detrás de una sirena; frecuencia del eco

### 1) Sirena quieta

$$
\lambda_0=\frac{v}{f_s}
=\frac{340}{300}
=1.133\,\mathrm m.
$$

### 2) Sirena en movimiento

Durante un período de emisión $T_s=1/f_s$, el sonido avanza $vT_s$ y la fuente $v_sT_s$. Hacia delante, la fuente alcanza al frente previo; detrás, se aleja de él:

$$
\lambda_{\mathrm{delante}}=\frac{v-v_s}{f_s}
=\frac{340-30}{300}
=1.033\,\mathrm m,
$$

$$
\lambda_{\mathrm{detrás}}=\frac{v+v_s}{f_s}
=\frac{340+30}{300}
=1.233\,\mathrm m.
$$

La primera es menor que la longitud de onda en reposo y la posterior es mayor.

### 3) Eco recibido por el conductor

Separamos el trayecto en dos cambios Doppler.

**Ida: la pared recibe el sonido de la fuente que se acerca.**

$$
f_{\mathrm{pared}}=f_s\frac{v}{v-v_s}
=300\frac{340}{340-30}
=329.0\,\mathrm{Hz}.
$$

La pared está quieta, por eso refleja esa misma frecuencia en su marco.

**Vuelta: la fuente se acerca a la onda reflejada.**

$$
f_{\mathrm{eco}}=f_{\mathrm{pared}}\frac{v+v_s}{v}
=329.0\frac{340+30}{340}
=358.1\,\mathrm{Hz}.
$$

Al multiplicar las dos etapas:

$$
f_{\mathrm{eco}}=f_s\frac{v+v_s}{v-v_s}.
$$

**Control:** el eco supera los $300\,\mathrm{Hz}$ porque la sirena se acerca a la pared y luego también se acerca a la onda reflejada.

---

## 27. Fuente y observador en movimiento simultáneo

### Signos respecto del aire

La fuente se aleja, por lo que $v_s=-45\,\mathrm{m/s}$. El receptor se mueve hacia la fuente, por lo que $v_o=+15\,\mathrm{m/s}$. Usamos la fórmula general:

$$
f_{\mathrm{obs}}=f_s\frac{v+v_o}{v-v_s}.
$$

### Sustitución

$$
f_{\mathrm{obs}}
=300\frac{340+15}{340-(-45)}
=300\frac{355}{385}
=276.6\,\mathrm{Hz}.
$$

### Interpretación

El receptor que se acerca encuentra más frentes por segundo, lo que eleva la frecuencia respecto del caso de receptor quieto. Sin embargo, la fuente que se aleja estira los frentes con más fuerza relativa: el denominador pasa de $340$ a $385\,\mathrm{m/s}$. Ese efecto domina y el resultado final queda por debajo de los $300\,\mathrm{Hz}$ emitidos.

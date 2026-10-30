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

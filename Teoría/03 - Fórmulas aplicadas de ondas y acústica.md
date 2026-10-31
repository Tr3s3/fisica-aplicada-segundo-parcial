---
tags: [fisica-aplicada, teoria, formulas, ondas-acustica]
---

# Fórmulas aplicadas — Ondas mecánicas y acústica

**Volver al módulo:** [[Teoría/03 - Ondas y acústica]] · **Significado físico:** [[Teoría/03 - Conceptos de ondas y acústica]] · **Práctica:** [[Ejercicios/03 - Ondas y acústica]]

> [!important] Notación de esta hoja
> $v$ es rapidez de propagación de la onda; $u$ es velocidad local de una partícula del medio; $s$ es desplazamiento de esa partícula; $\Delta p$ es variación acústica de presión. En Doppler, $v_s$ y $v_o$ son rapidez con signo de fuente y observador respecto del aire.

## Mapa de selección

| Buscas… | Empieza con… |
|---|---|
| $T$, $f$, $\lambda$, $k$, $\omega$ | $v=\lambda f$, $k=2\pi/\lambda$, $\omega=2\pi f$ |
| Rapidez del sonido según el medio | $v=\sqrt{B/\rho}$, $\sqrt{\gamma RT/M}$ o $\sqrt{Y/\rho}$ |
| Desplazamiento desde presión | $\Delta p_{\max}=Bk s_{\max}=\rho v\omega s_{\max}$ |
| Intensidad desde presión | $I=p_{\max}^2/(2\rho v)$ o $I=p_{\mathrm{rms}}^2/(\rho v)$ |
| Potencia o nivel según la distancia | $I=P_{\mathrm{ac}}/(4\pi r^2)$ |
| Nivel sonoro | $\beta=10\log_{10}(I/I_0)$ |
| Refuerzo o cancelación | Diferencia de caminos y relación con $\lambda$ |
| Frecuencia recibida | Doppler; define movimientos respecto del medio |
| Eco que vuelve a una fuente móvil | Dos etapas Doppler separadas |

## 1. Parámetros y función de una onda armónica

El patrón avanza una longitud de onda durante un período. De ahí sale la relación entre rapidez, longitud y frecuencia:

$$
v=\frac{\lambda}{T}=\lambda f,\qquad T=\frac1f.
$$

La fase permite ubicar el patrón en espacio y tiempo:

$$
s(x,t)=s_{\max}\cos(kx-\omega t+\phi_0),
\qquad
k=\frac{2\pi}{\lambda},
\qquad
\omega=2\pi f.
$$

- $k$ se mide en $\mathrm{rad/m}$ y describe el cambio espacial de fase.
- $\omega$ se mide en $\mathrm{rad/s}$ y describe el cambio temporal de fase.
- $kx-\omega t$ representa una onda que avanza hacia $+x$. Con $kx+\omega t$ avanza hacia $-x$.
- $s_{\max}$ es amplitud de desplazamiento. No debe confundirse con la amplitud de presión.

La rapidez local de las partículas se obtiene derivando el desplazamiento respecto del tiempo:

$$
u(x,t)=\frac{\partial s}{\partial t},
\qquad
u_{\max}=\omega s_{\max}.
$$

$u$ oscila; $v$ describe el avance de la fase. En general no son iguales.

Si se conoce el intervalo audible humano aproximado $20$–$20\,000\,\mathrm{Hz}$ y la rapidez del sonido, el rango de longitudes de onda sale de $\lambda=v/f$. La frecuencia menor produce la longitud de onda mayor.

## 2. Rapidez de propagación según el material

Usa la ecuación correspondiente al tipo de medio. Rigidez más alta tiende a acelerar la transmisión; más densidad aumenta la inercia.

| Medio o modelo | Rapidez | Datos |
|---|---|---|
| Fluido (líquido o gas, si se conocen sus propiedades) | $v=\sqrt{B/\rho}$ | $B$: módulo volumétrico en Pa; $\rho$: densidad en $\mathrm{kg/m^3}$ |
| Gas ideal | $v=\sqrt{\gamma p/\rho}=\sqrt{\gamma RT/M}$ | $\gamma=C_p/C_v$; $T$ en K; $M$ en kg/mol |
| Varilla delgada | $v\approx\sqrt{Y/\rho}$ | $Y$: módulo de Young en Pa; $\rho$: densidad del material |
| Cuerda tensa, si el problema la incluye | $v=\sqrt{F_T/\mu}$ | $F_T$: tensión; $\mu$: masa por unidad de longitud |

### De dónde sale la raíz de rigidez sobre inercia

Para un pequeño elemento de fluido de sección $A$ y largo $\Delta x$, una diferencia de presión produce una fuerza neta aproximada $-A\Delta x\,\partial(\Delta p)/\partial x$. Su masa es $\rho A\Delta x$. Aplicando Newton:

$$
\rho\frac{\partial^2s}{\partial t^2}
=-\frac{\partial(\Delta p)}{\partial x}.
$$

La elasticidad del fluido da $\Delta p=-B\,\partial s/\partial x$. Al reemplazar:

$$
\frac{\partial^2s}{\partial t^2}
=\frac{B}{\rho}\frac{\partial^2s}{\partial x^2}.
$$

La ecuación de onda estándar tiene coeficiente $v^2$ delante de la derivada espacial. Por comparación, $v^2=B/\rho$. La rapidez aumenta si el medio ofrece una respuesta elástica fuerte y disminuye si la masa por volumen es grande.

En gases, la compresión durante el paso de una onda sonora es aproximadamente adiabática: $pV^\gamma=\text{constante}$. Para pequeños cambios eso da $B=\gamma p$, y entonces $v=\sqrt{\gamma p/\rho}$. Con la ecuación del gas ideal $p/\rho=RT/M$ se obtiene la forma con $T$ y masa molar:

$$
v=\sqrt{\frac{\gamma RT}{M}}.
$$

No uses temperatura Celsius ni $M$ en gramos por mol dentro de esa expresión. Si el ejercicio entrega directamente $v$, úsala sin reconstruirla.

Al cruzar a otro medio la frecuencia se conserva, pero cambia la rapidez. Entonces cambia también la longitud de onda:

$$
f_{\mathrm{nuevo}}=f_{\mathrm{fuente}},
\qquad
\lambda_{\mathrm{nuevo}}=\frac{v_{\mathrm{nuevo}}}{f_{\mathrm{fuente}}}.
$$

### Caso del oído en la práctica

En el modelo simplificado del TP, la fuerza transmitida por los huesecillos se aplica sobre un área efectiva menor. Si se supone la misma fuerza, $F=pA$ da:

$$
p_2A_2=p_1A_1
\quad\Longrightarrow\quad
p_2=p_1\frac{A_1}{A_2}.
$$

Después, para el fluido del oído se usa su propia rapidez y densidad (o módulo volumétrico) en la conversión de presión a desplazamiento. Esta relación de áreas es la idealización del ejercicio; no representa todos los detalles del oído real.

## 3. De presión a desplazamiento: origen de la relación

La presión acústica se debe a la compresión o expansión local. Para desplazamientos pequeños, la deformación relativa a lo largo de $x$ es aproximadamente:

$$
\frac{\Delta V}{V}\approx\frac{\partial s}{\partial x}.
$$

El módulo volumétrico se define como resistencia a esa deformación:

$$
B=-\frac{\Delta p}{\Delta V/V}.
$$

El signo negativo expresa que reducir volumen produce aumento de presión. Por eso:

$$
\Delta p\approx-B\frac{\partial s}{\partial x}.
$$

Para $s=s_{\max}\cos(kx-\omega t)$:

$$
\Delta p=Bk s_{\max}\sin(kx-\omega t).
$$

El seno y el coseno están desfasados $\pi/2$ rad, es decir, $\lambda/4$. Una compresión máxima coincide con una presión acústica máxima, pero no con el máximo desplazamiento de las partículas.

Comparando amplitudes:

$$
\boxed{\Delta p_{\max}=Bk s_{\max}},
\qquad
\boxed{s_{\max}=\frac{\Delta p_{\max}}{Bk}}.
$$

Como $k=2\pi f/v$:

$$
s_{\max}=\frac{\Delta p_{\max}v}{2\pi fB}.
$$

En un fluido, $v^2=B/\rho$, de modo que $B=\rho v^2$ y $\omega=vk$. La relación equivalente es:

$$
\Delta p_{\max}=\rho v\omega s_{\max}
=\rho v u_{\max}.
$$

Esta forma es útil si se conoce la densidad del medio. Las dos formas dan el mismo resultado siempre que propiedades y amplitudes correspondan al mismo medio.

**Control dimensional:**

$$
[Bk]=\mathrm{Pa/m},
\qquad
\left[\frac{\Delta p_{\max}}{Bk}\right]=\mathrm m.
$$

## 4. Intensidad sonora a partir de la presión

La intensidad es potencia media por área. Para una onda sinusoidal progresiva:

$$
I=\langle\Delta p\,u\rangle.
$$

En la onda que avanza, presión y velocidad local de las partículas están en fase. Como el promedio de $\sin^2$ en un ciclo es $1/2$:

$$
I=\frac12\Delta p_{\max}u_{\max}.
$$

Usando $\Delta p_{\max}=\rho v u_{\max}$:

$$
\boxed{I=\frac{(\Delta p_{\max})^2}{2\rho v}}
\qquad\text{(presión de amplitud máxima).}
$$

Si el dato es presión eficaz:

$$
p_{\mathrm{rms}}=\frac{\Delta p_{\max}}{\sqrt2},
\qquad
\boxed{I=\frac{p_{\mathrm{rms}}^2}{\rho v}}.
$$

No uses el factor $2$ otra vez con $p_{\mathrm{rms}}$. Si no se especifica RMS o eficaz, en los ejercicios de esta guía el símbolo $p_{\max}$ indica amplitud máxima.

### Consecuencia para ondas de igual intensidad

En un mismo medio, $I=p_{\max}^2/(2\rho v)$. Si dos ondas tienen la misma intensidad, tienen igual amplitud máxima de presión. En cambio:

$$
s_{\max}=\frac{p_{\max}}{\rho v\,2\pi f}
\quad\Longrightarrow\quad
s_{\max}\propto\frac1f
\quad\text{si $I$, $\rho$ y $v$ son iguales.}
$$

Por eso una onda de $20\,\mathrm{Hz}$ y una de $1000\,\mathrm{Hz}$ con igual intensidad tienen la misma amplitud de presión, pero la de menor frecuencia necesita mayor amplitud de desplazamiento.

## 5. Potencia acústica, distancia y ecos de sonar

Para una fuente puntual ideal que emite isotrópicamente, la potencia cruza la superficie esférica de radio $r$:

$$
I=\frac{P_{\mathrm{ac}}}{4\pi r^2},
\qquad
P_{\mathrm{ac}}=4\pi r^2I.
$$

La fórmula supone que no hay pérdidas significativas, absorción ni obstáculos. Al duplicar $r$, la intensidad queda dividida por cuatro.

En un sonar que emite un pulso y mide el eco, si el objeto está a distancia $d$ y el tiempo total de ida y vuelta es $\Delta t$:

$$
2d=v\Delta t,
\qquad
d=\frac{v\Delta t}{2}.
$$

El factor $2$ aparece porque el pulso recorre el trayecto hasta el objeto y el regreso al detector. Luego, si se pide la longitud de onda de una frecuencia $f$, se calcula $\lambda=v/f$.

## 6. Nivel sonoro, decibeles y fuentes

El nivel compara la intensidad medida con una referencia:

$$
\boxed{\beta=10\log_{10}\left(\frac{I}{I_0}\right)},
\qquad
I_0=1.0\times10^{-12}\,\mathrm{W/m^2}.
$$

La razón dentro del logaritmo no tiene unidades. Para despejar:

$$
\boxed{I=I_0\,10^{\beta/10}}.
$$

Cambios de nivel:

$$
\Delta\beta=10\log_{10}\left(\frac{I_2}{I_1}\right).
$$

Así se obtienen reglas útiles:

- $I_2=10I_1$: $+10\,\mathrm{dB}$.
- $I_2=2I_1$: $+3.01\,\mathrm{dB}$.
- $I_2=I_1/4$: $-6.02\,\mathrm{dB}$.

Si las fuentes son independientes:

$$
I_{\mathrm{tot}}=\sum_i I_i,
\qquad
\beta_{\mathrm{tot}}=10\log_{10}\left(\frac{I_{\mathrm{tot}}}{I_0}\right).
$$

Para $N$ fuentes independientes iguales:

$$
\beta_{\mathrm{tot}}=\beta_1+10\log_{10}N.
$$

Si el problema compara amplitudes de presión en el mismo medio, y las señales son ondas progresivas comparables, $I\propto p^2$ permite escribir:

$$
\Delta\beta=20\log_{10}\left(\frac{p_2}{p_1}\right).
$$

Esta regla compara presiones; no reemplaza la suma de intensidades para fuentes incoherentes ni la suma de ondas para fuentes coherentes.

## 7. Superposición e interferencia

Para dos fuentes coherentes que emiten en fase, calcula primero la diferencia de caminos en el punto de observación:

$$
\Delta r=|r_A-r_B|.
$$

Después usa la condición de fase:

| Resultado en el punto | Diferencia de camino | Frecuencias si $\lambda=v/f$ |
|---|---|---|
| Constructiva | $\Delta r=m\lambda$ | $f=mv/\Delta r$, $m=1,2,\ldots$; si $\Delta r=0$, es constructiva para toda frecuencia |
| Destructiva | $\Delta r=(m+\tfrac12)\lambda$ | $f=(m+\tfrac12)v/\Delta r$, $m=0,1,2,\ldots$ |

Si las fuentes inicialmente tienen una fase relativa distinta de cero, hay que incluir ese desfase; las reglas de esta tabla suponen que emiten en fase.

Para sonido reflejado por una pared rígida, la presión reflejada está en fase con la presión incidente en la pared. Los nodos de presión se sitúan idealmente en:

$$
x=\frac{(2m+1)\lambda}{4},
\qquad m=0,1,2,\ldots
$$

desde la pared. Para aplicar la condición se necesita la longitud de onda en el medio donde ocurre la reflexión.

## 8. Doppler acústico: fuente y observador

Para propagación colineal en un medio en reposo:

$$
\boxed{
f_{\mathrm{obs}}=f_s\frac{v+v_o}{v-v_s}
}
$$

Convención usada:

- $v>0$ es la rapidez del sonido respecto del aire.
- $v_o>0$ si el observador se mueve hacia la fuente; $v_o<0$ si se aleja.
- $v_s>0$ si la fuente se mueve hacia el observador; $v_s<0$ si se aleja.
- $f_s$ es la frecuencia emitida; $f_{\mathrm{obs}}$ la recibida.

Las expresiones de esta unidad suponen movimiento sobre la línea fuente-observador y rapidez de la fuente menor que la rapidez del sonido. En las situaciones del parcial y del TP, las fuentes cumplen esa condición.

### Por qué la fuente va abajo y el observador arriba

Durante un período de emisión $T_s=1/f_s$, el sonido avanza $vT_s$. Si la fuente se mueve hacia el observador a $v_s$, la fuente avanza en ese mismo tiempo y reduce el espaciamiento delantero:

$$
\lambda_{\mathrm{delante}}=(v-v_s)T_s=\frac{v-v_s}{f_s}.
$$

Si se aleja, con nuestra convención $v_s<0$ y el denominador $v-v_s$ crece; detrás de una fuente que se aleja la longitud de onda es $(v+|v_s|)/f_s$.

El observador no altera los frentes ya formados en el aire. Sí cambia la rapidez con que los encuentra: $v+v_o$. Por tanto:

$$
f_{\mathrm{obs}}=
\frac{\text{rapidez de encuentro}}{\text{separación entre frentes}}
=\frac{v+v_o}{(v-v_s)/f_s}.
$$

| Situación | Signos | Tendencia |
|---|---|---|
| Fuente se acerca; observador quieto | $v_s>0$, $v_o=0$ | $f_{\mathrm{obs}}>f_s$ |
| Fuente se aleja; observador quieto | $v_s<0$, $v_o=0$ | $f_{\mathrm{obs}}<f_s$ |
| Observador se acerca; fuente quieta | $v_s=0$, $v_o>0$ | $f_{\mathrm{obs}}>f_s$ |
| Observador se aleja; fuente quieta | $v_s=0$, $v_o<0$ | $f_{\mathrm{obs}}<f_s$ |

### Eco en una pared quieta: dos aplicaciones

Si una fuente móvil se aproxima a una pared fija:

1. La pared recibe la frecuencia Doppler causada por la fuente:
   $$
   f_{\mathrm{pared}}=f_s\frac{v}{v-v_s}.
   $$
2. La pared refleja esa misma frecuencia en su marco. La fuente se mueve hacia la onda reflejada y actúa como observador:
   $$
   f_{\mathrm{eco}}=f_{\mathrm{pared}}\frac{v+v_s}{v}.
   $$

Al combinar:

$$
\boxed{f_{\mathrm{eco}}=f_s\frac{v+v_s}{v-v_s}}.
$$

Con fuente que se aproxima, el eco debe sonar más agudo que la sirena original. La fórmula presupone pared quieta, movimiento en la línea fuente-pared y rapidez de la fuente menor que la del sonido.

## 9. Errores de planteo que esta hoja ayuda a evitar

| Confusión | Revisión |
|---|---|
| Usar $v$ para la oscilación de las moléculas | Usa $u=\partial s/\partial t$ para las partículas; $v=\lambda f$ para la onda |
| Usar la presión atmosférica como amplitud sonora | La amplitud es $\Delta p$ alrededor de la presión de equilibrio |
| Usar $p_{\max}$ en la fórmula RMS o viceversa | $I=p_{\max}^2/(2\rho v)$; $I=p_{\mathrm{rms}}^2/(\rho v)$ |
| Calcular rapidez del sonido con la fórmula de otro medio | Elige fluido, gas ideal, varilla o el dato proporcionado |
| Sumar niveles en dB | Suma intensidades de fuentes incoherentes y convierte el total |
| Usar Doppler sin un esquema | Mide ambas velocidades respecto del aire y define acercamiento |
| Aplicar una sola fórmula al eco de una pared | Separa frecuencia recibida por la pared y frecuencia recibida por la fuente |
| Confundir intensidad y potencia | La intensidad se mide en $\mathrm{W/m^2}$; la potencia en W |

## Fuentes cotejadas

- [Presentación de ondas y sonido](zotero://select/library/items/WFMW87CP): rapidez por medio, intensidad, escala de nivel y efecto Doppler, PDF pp. 12–22.
- [Práctica de sonido 2021](zotero://select/library/items/ZFCVVKE5): ejercicios 1–17. Abarca presión-desplazamiento, oído, sonar, rapidez en materiales, intensidad, potencia, decibeles, interferencia, Doppler y eco.
- Los recortes de sonar e interferencia están en [[Teoría/03 - Conceptos de ondas y acústica]].

## Autoevaluación de aplicación

Antes de desplegar la respuesta, anota el modelo y explica por qué corresponde.

**1. Una onda de $500\,\mathrm{Hz}$ se propaga a $340\,\mathrm{m/s}$. ¿Cómo obtienes $\lambda$ y $k$?**

> [!success]- Mostrar explicación
> $\lambda=v/f=0.680\,\mathrm m$ y $k=2\pi/\lambda\approx9.24\,\mathrm{rad/m}$. $v$ es rapidez de la onda.

**2. Si una misma intensidad en aire corresponde a ondas de $20\,\mathrm{Hz}$ y $1000\,\mathrm{Hz}$, ¿qué amplitudes son iguales y cuál cambia?**

> [!success]- Mostrar explicación
> Como el medio no cambia, igual intensidad implica igual amplitud de presión. La amplitud de desplazamiento es inversamente proporcional a $f$, así que la onda de $20\,\mathrm{Hz}$ desplaza las partículas 50 veces más.

**3. Una fuente puntual mantiene su potencia y el oyente duplica la distancia. ¿Qué pasa con $I$ y $\beta$?**

> [!success]- Mostrar explicación
> $I\propto1/r^2$, por lo que la intensidad queda en una cuarta parte. El cambio de nivel es $10\log_{10}(1/4)\approx-6.02\,\mathrm{dB}$.

**4. Dos parlantes en fase tienen diferencia de camino $1.5\,\mathrm m$. ¿Qué condición corresponde a un mínimo ideal?**

> [!success]- Mostrar explicación
> Para interferencia destructiva, $\Delta r=(m+\tfrac12)\lambda$. Se despeja la longitud de onda y, si hace falta, se usa $f=v/\lambda$. Si las fuentes no emiten en fase, debe incluirse su fase relativa.

**5. Una ambulancia se aleja de un receptor quieto. ¿Qué signos se usan?**

> [!success]- Mostrar explicación
> Con esta convención, $v_s<0$ y $v_o=0$. El denominador $v-v_s$ crece, por lo que la frecuencia recibida resulta menor que la emitida.

**6. ¿Por qué un eco que vuelve a una fuente que se acerca a una pared tiene dos factores Doppler?**

> [!success]- Mostrar explicación
> La fuente móvil cambia la frecuencia que recibe primero la pared; después la fuente móvil recibe la onda reflejada como observadora que se acerca. Se calcula cada tramo con su emisor y receptor y luego se multiplican ambos factores.

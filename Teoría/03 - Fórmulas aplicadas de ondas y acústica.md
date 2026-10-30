---
tags: [fisica-aplicada, teoria, formulas, ondas-acustica]
---

# Fórmulas aplicadas — Ondas y acústica

**Volver al módulo:** [[Teoría/03 - Ondas y acústica]] · **Conceptos:** [[Teoría/03 - Conceptos de ondas y acústica]] · **Práctica:** [[Ejercicios/03 - Ondas y acústica]]

> [!important] Antes de sustituir
> Dibuja el medio y la dirección de propagación; convierte a SI; identifica si la presión dada es una amplitud máxima o eficaz. Para Doppler, las velocidades se miden respecto del medio.

## 1. Parámetros de una onda sinusoidal

$$
T=\frac{1}{f},\qquad
\omega=2\pi f=\frac{2\pi}{T},\qquad
k=\frac{2\pi}{\lambda},\qquad
v=\lambda f=\frac{\omega}{k}.
$$

- $T$ en segundos; $f$ en hertz; $\lambda$ en metros; $v$ en $\mathrm{m/s}$.
- $\omega$ es la frecuencia angular en $\mathrm{rad/s}$.
- $k$ es el número de onda en $\mathrm{rad/m}$.
- La igualdad $v=\lambda f$ expresa que en un período $T$ la forma de onda avanza una longitud $\lambda$: $v=\lambda/T$.

Para una onda que avanza hacia $+x$ puede escribirse, por ejemplo,
$$
s(x,t)=s_{\max}\cos(kx-\omega t).
$$
El signo entre $kx$ y $\omega t$ fija el sentido de avance; cambiarlo representa una onda que viaja en el sentido contrario.

## 2. Rapidez del sonido en cada medio

Usa una relación elástica solo si el ejercicio entrega o pide esas propiedades. Si ya te dan $v$, utiliza el dato.

$$
v_{\mathrm{fluido}}=\sqrt{\frac{B}{\rho}},\qquad
v_{\mathrm{gas}}=\sqrt{\frac{\gamma p}{\rho}}
=\sqrt{\frac{\gamma R T}{M}},\qquad
v_{\mathrm{varilla}}\approx\sqrt{\frac{Y}{\rho}}.
$$

- $B$: módulo volumétrico, en Pa; $\rho$: densidad, en $\mathrm{kg/m^3}$.
- Para el gas ideal, $\gamma=C_p/C_v$, $p$ es presión de equilibrio, $T$ temperatura absoluta, $R=8.314\,\mathrm{J/(mol\,K)}$ y $M$ masa molar en $\mathrm{kg/mol}$.
- $Y$ es el módulo de Young del material de una varilla delgada.

No uses Celsius en una ecuación con temperatura absoluta. La expresión de gas ideal se obtiene usando $p/\rho=RT/M$. En aire a temperatura ambiente el valor suele estar cerca de $340\,\mathrm{m/s}$; respeta el valor que indique el problema.

## 3. De presión a desplazamiento de las partículas

Para desplazamientos pequeños en un fluido:

$$
\frac{\Delta V}{V}\approx\frac{\partial s}{\partial x},
\qquad
\Delta p=-B\frac{\Delta V}{V}
\approx-B\frac{\partial s}{\partial x}.
$$

Si $s=s_{\max}\cos(kx-\omega t)$, al derivar respecto de $x$ se obtiene una variación de presión sinusoidal desfasada un cuarto de ciclo. Comparando amplitudes:

$$
\Delta p_{\max}=B k s_{\max},
\qquad
s_{\max}=\frac{\Delta p_{\max}}{Bk}
=\frac{\Delta p_{\max}v}{2\pi fB}.
$$

**Cuándo sirve:** el enunciado da la amplitud de presión, el módulo volumétrico, la frecuencia y la rapidez y pide el desplazamiento. No sumes la presión atmosférica: $\Delta p_{\max}$ es la variación alrededor de ella.

**Control dimensional:** $Bk$ tiene unidades $\mathrm{Pa/m}$; por eso $\Delta p_{\max}/(Bk)$ queda en metros.

## 4. Intensidad acústica a partir de la presión

Para una onda sinusoidal progresiva, usando amplitud máxima de presión:

$$
I=\frac{(\Delta p_{\max})^2}{2\rho v}.
$$

Si el enunciado informa presión eficaz $p_{\mathrm{rms}}=\Delta p_{\max}/\sqrt{2}$, usa la forma equivalente:

$$
I=\frac{p_{\mathrm{rms}}^2}{\rho v}.
$$

No introduzcas el factor 2 dos veces. La intensidad media se mide en $\mathrm{W/m^2}$.

Si el sonido de una fuente puntual se reparte uniformemente en todas direcciones:

$$
I(r)=\frac{P_{\mathrm{ac}}}{4\pi r^2}.
$$

Esta última relación supone propagación esférica sin absorción apreciable ni obstáculos.

## 5. Nivel sonoro y suma de fuentes

$$
\beta=10\log_{10}\left(\frac{I}{I_0}\right),
\qquad
I_0=1.0\times10^{-12}\,\mathrm{W/m^2}.
$$

El argumento del logaritmo es una razón sin unidades. Para despejar intensidad:

$$
I=I_0\,10^{\beta/10}.
$$

Para fuentes independientes:

$$
I_{\mathrm{tot}}=\sum_i I_i,
\qquad
\beta_{\mathrm{tot}}=10\log_{10}\left(\frac{I_{\mathrm{tot}}}{I_0}\right).
$$

Con $N$ fuentes iguales de intensidad $I$:
$$
I_{\mathrm{tot}}=NI,\qquad
\beta_{\mathrm{tot}}=\beta_1+10\log_{10}N.
$$
Dos fuentes iguales aumentan el nivel en $10\log_{10}2=3.01\,\mathrm{dB}$.

## 6. Efecto Doppler: fórmula y signos

Para sonido en un medio en reposo:

$$
f_{\mathrm{obs}}
=f_{\mathrm{fuente}}
\frac{v+v_o}{v-v_s}.
$$

Convención de esta guía:

- $v>0$: rapidez del sonido respecto del medio.
- $v_o>0$ si el observador se mueve **hacia la fuente**; $v_o<0$ si se aleja.
- $v_s>0$ si la fuente se mueve **hacia el observador**; $v_s<0$ si se aleja.
- $f_{\mathrm{fuente}}$ es la frecuencia emitida; $f_{\mathrm{obs}}$ la recibida.

| Caso | Sustitución | Resultado esperado |
|---|---|---|
| Fuente se acerca; observador quieto | $v_o=0$, $v_s>0$ | $f_{\mathrm{obs}}>f_{\mathrm{fuente}}$ |
| Fuente se aleja; observador quieto | $v_o=0$, $v_s<0$ | $f_{\mathrm{obs}}<f_{\mathrm{fuente}}$ |
| Observador se acerca; fuente quieta | $v_o>0$, $v_s=0$ | $f_{\mathrm{obs}}>f_{\mathrm{fuente}}$ |
| Observador se aleja; fuente quieta | $v_o<0$, $v_s=0$ | $f_{\mathrm{obs}}<f_{\mathrm{fuente}}$ |

### Por qué fuente y observador ocupan lugares distintos

Una fuente móvil cambia la separación de los frentes en el medio. Delante de una fuente que se acerca, durante un período $T_s=1/f_s$ el frente avanza $vT_s$ mientras la fuente avanza $v_sT_s$; por tanto,
$$
\lambda'=(v-v_s)T_s=\frac{v-v_s}{f_s}.
$$
El observador móvil intercepta esos frentes con rapidez relativa $v+v_o$. Así:
$$
f_{\mathrm{obs}}=\frac{v+v_o}{\lambda'}
=f_s\frac{v+v_o}{v-v_s}.
$$
Esto justifica por qué $v_o$ va en el numerador y $v_s$ en el denominador. La figura está en [[Teoría/03 - Ondas y acústica#Efecto Doppler: separar el papel de la fuente y del observador]].

### Secuencia de decisión

1. Dibuja fuente, observador, aire y sentido de la onda que viaja hasta el receptor.
2. Escribe $v_o$ y $v_s$ respecto del aire, con signo.
3. Sustituye los signos en la fórmula general; no memorices fórmulas separadas sin indicar el caso.
4. Revisa si acercarse sube la frecuencia o alejarse la baja.
5. Para un eco en una pared fija, separa las etapas: la pared recibe el sonido de la fuente móvil y luego refleja esa frecuencia; la fuente móvil recibe el eco como observador en movimiento.

## Errores frecuentes

| Error | Corrección |
|---|---|
| Confundir $s_{\max}$ con $\Delta p_{\max}$ | Son amplitudes de magnitudes distintas; usa $Bks_{\max}=\Delta p_{\max}$. |
| Sumar $p_{\mathrm{atm}}$ a la amplitud de presión | La amplitud es una variación alrededor de la presión de equilibrio. |
| Ingresar una presión eficaz como amplitud máxima | Identifica RMS; las dos fórmulas de intensidad difieren por el factor 2. |
| Sumar decibeles de dos máquinas | Suma intensidades y convierte el total una sola vez. |
| Poner la rapidez de la fuente en el numerador Doppler | La fuente altera la longitud de onda; el observador altera la tasa de encuentro. |
| Tomar la velocidad de la ambulancia respecto de la calle sin pensar en el aire | En Doppler acústico las velocidades se miden respecto del medio. |
| Esperar que $v=\lambda f$ dé la rapidez de las partículas | Da la rapidez de propagación de fase de la onda. |

## Fuentes cotejadas

- [Presentación de ondas y sonido](zotero://select/library/items/WFMW87CP): rapidez en gases, líquidos y sólidos, PDF pp. 13–14; intensidad, p. 15; nivel, pp. 16–17; Doppler, pp. 18–22.
- [Práctica de sonido 2021](zotero://select/library/items/ZFCVVKE5): ejercicios 1, 6–10 y 13–17.
- [Modelos 2023, 2024 y 2025](zotero://select/library/items/YIXUYDMC), [2024](zotero://select/library/items/HQ9E54FP) y [2025](zotero://select/library/items/DHM5X7QD): familias de problemas de nivel sonoro, Doppler y presión-desplazamiento.

---
tags: [fisica-aplicada, teoria, ondas-acustica]
---

# Teoría — Ondas y acústica

**Recorrido:** [[Teoría/00 - Mapa y formulario general|Mapa general]] → [[Ejercicios/03 - Ondas y acústica|Práctica]] → [[Resoluciones/03 - Ondas y acústica|Resoluciones modelo]]

## Conceptos y fórmulas

Para una onda sinusoidal:

$$
v=\lambda f,\qquad
k=\frac{2\pi}{\lambda}=\frac{2\pi f}{v},\qquad
\omega=2\pi f.
$$

### Presión y desplazamiento del aire

El sonido es una onda longitudinal: las partículas del aire oscilan paralelas a la propagación. Para amplitud de presión $\Delta p_{max}$ y desplazamiento máximo $s_{max}$:

$$
\Delta p_{max}=Bks_{max}
\quad\Rightarrow\quad
s_{max}=\frac{\Delta p_{max}}{Bk}
=\frac{\Delta p_{max}v}{2\pi fB}.
$$

La relación surge de que la compresión máxima es $ks_{max}$ y el cambio de presión es el módulo volumétrico $B$ por esa deformación. La amplitud de presión es una variación alrededor de la presión ambiente; no se suma la presión atmosférica.

![[imagenes/sonido-longitudinal.svg]]

### Intensidad y nivel sonoro

Para una onda sonora sinusoidal:

$$
I=\frac{(\Delta p_{max})^2}{2\rho v}.
$$

El nivel sonoro es:

$$
\beta=10\log_{10}\left(\frac I{I_0}\right),\qquad
I_0=10^{-12}\,\mathrm{W/m^2}.
$$

Fuentes independientes: suma sus intensidades antes de pasar a decibeles. Dos fuentes idénticas duplican $I$ y aumentan el nivel en $10\log_{10}2\approx3.01\,\mathrm{dB}$.

### Efecto Doppler

Con el medio en reposo:

$$
f'=f\frac{v_{snd}+v_o}{v_{snd}-v_s}.
$$

Usa $v_o>0$ si el observador se acerca y $v_o<0$ si se aleja; $v_s>0$ si la fuente se acerca y $v_s<0$ si se aleja. Dibuja fuente, observador y aire. Acercarse debe elevar la frecuencia recibida; alejarse debe reducirla.

![[imagenes/doppler-sonido.svg]]

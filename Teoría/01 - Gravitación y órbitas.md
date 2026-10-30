---
tags: [fisica-aplicada, teoria, gravitacion]
---

# Teoría — Gravitación y órbitas

**Recorrido:** [[Teoría/00 - Mapa y formulario general|Mapa general]] → [[Ejercicios/01 - Gravitación y órbitas|Práctica]] → [[Resoluciones/01 - Gravitación y órbitas|Resoluciones modelo]]

## Conceptos y fórmulas

### Fuerza, campo y peso

Para dos masas separadas por $r$:

$$
F=G\frac{m_1m_2}{r^2},\qquad
g=G\frac{M}{r^2},\qquad
W=mg.
$$

El campo apunta hacia la masa que lo produce. Para varias fuentes, suma los vectores campo:

$$
\vec g(P)=\sum_i G\frac{M_i}{r_i^2}\,\hat r_{P\to i},
\qquad
\vec F_{prueba}=m_{prueba}\vec g(P).
$$

En una distribución simétrica, separa cada campo en componentes. Las horizontales pueden cancelarse y las verticales sumarse. La aceleración no depende de la masa de prueba.

![[imagenes/campo-gravitatorio.svg]]

A altura $h$ sobre un planeta de radio $R$, la distancia al centro es $r=R+h$. Como $g_0=GM/R^2$:

$$
g(h)=g_0\left(\frac{R}{R+h}\right)^2,\qquad
W_h=W_0\left(\frac{R}{R+h}\right)^2.
$$

La masa no cambia; el peso sí. Si te dan el peso orbital y piden el de superficie:

$$
W_0=W_h\left(\frac{R+h}{R}\right)^2.
$$

Por ejemplo, si $h=0.35R$, entonces $r=1.35R$. La altura $h$ no es el radio orbital $r$.

### Órbita circular, energía y escape

![[imagenes/orbita-satelite.svg]]

Iguala fuerza gravitatoria y centrípeta:

$$
G\frac{Mm}{r^2}=m\frac{v^2}{r}
\quad\Rightarrow\quad
v_{orb}=\sqrt{\frac{GM}{r}}.
$$

La masa del satélite se cancela. El período:

$$
T=\frac{2\pi r}{v}
=2\pi\sqrt{\frac{r^3}{GM}}.
$$

La energía potencial es $U=-GMm/r$. En órbita circular, $K=GMm/(2r)$, así que:

$$
E_{total}=K+U=-\frac{GMm}{2r}.
$$

Es negativa porque el satélite está ligado gravitatoriamente. Para escapar desde la distancia inicial $r$, la energía final mínima es cero:

$$
\frac12mv_{esc}^2-\frac{GMm}{r}=0
\quad\Rightarrow\quad
v_{esc}=\sqrt{\frac{2GM}{r}}.
$$

Usa $r=R$ si parte de la superficie y su radio orbital si parte de una órbita.

### Tercera ley de Kepler

Para cuerpos que orbitan la misma masa central:

$$
\frac{T^2}{r^3}=\text{constante},\qquad
r_2=r_1\left(\frac{T_2}{T_1}\right)^{2/3}.
$$

Si se conocen $T$ y $r$:

$$
M=\frac{4\pi^2r^3}{GT^2}.
$$

Al comparar planetas usando años y UA, la Tierra vale $T=1$ y $r=1$.

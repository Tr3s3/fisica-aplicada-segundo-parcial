---
tags: [fisica-aplicada, teoria, conceptos, ondas-em]
---

# Conceptos de ondas electromagnéticas

[[Teoría/04 - Ondas electromagnéticas|← Índice del módulo]] · [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|Formulario aplicado]]

## 1. Qué se propaga

Una onda electromagnética es una perturbación de los campos eléctrico $\vec E$ y magnético $\vec B$ que avanza por el espacio. Las ecuaciones de Maxwell describen cómo un campo magnético variable puede generar un campo eléctrico y cómo un campo eléctrico variable puede generar un campo magnético. Esa interacción permite que la perturbación avance incluso en el vacío: no necesita aire, cuerda ni otro medio material.

Esto la distingue del sonido, que necesita un medio cuyas partículas oscilen. En la onda electromagnética, lo que oscila son los propios campos.

## 2. Geometría de una onda plana en el vacío

En cada punto de una onda plana, los tres sentidos relevantes son perpendiculares:

$$
\vec E\perp\vec B,\qquad
\vec E\perp\hat n,\qquad
\vec B\perp\hat n,
$$

donde $\hat n$ es un vector unitario que apunta en la dirección de propagación. Por eso, si se conocen dos sentidos, el tercero no se elige al azar: queda fijado por la regla de la mano derecha.

La dirección de transporte de energía también coincide con $\vec E\times\vec B$. Esta comprobación es esencial al escribir ecuaciones vectoriales: una amplitud positiva siempre se entiende en el sentido del vector unitario escrito delante.

![[imagenes/onda-electromagnetica.svg]]

## 3. Frecuencia, longitud de onda y rapidez

La frecuencia $f$ cuenta cuántos ciclos pasan por un punto cada segundo. La longitud de onda $\lambda$ es la distancia entre puntos consecutivos que están en la misma fase. En el vacío, la onda se propaga a la rapidez de la luz $c$; en un período $T$, recorre una longitud de onda:

$$
c=\frac{\lambda}{T}=\lambda f.
$$

La frecuencia la fija la fuente. Si la onda sigue en el vacío, una frecuencia mayor corresponde a una longitud de onda menor.

## 4. Campos que oscilan juntos

Para una onda sinusoidal plana en el vacío, los campos eléctrico y magnético alcanzan sus máximos y cruzan cero en los mismos lugares y momentos: están en fase. Sus amplitudes no son independientes. La relación

$$
E_{max}=cB_{max}
$$

significa que el valor numérico de $E_{max}/B_{max}$ es la rapidez de propagación. No significa que $E$ y $B$ tengan la misma unidad: $E$ se mide en $\mathrm{V/m}$ y $B$ en teslas.

## 5. Leer el sentido desde la fase

Para una onda que depende solo de $x$, una fase de la forma $kx-\omega t$ se desplaza hacia $+x$. Se ve manteniendo fija la fase:

$$
kx-\omega t=\text{constante}
\quad\Longrightarrow\quad
\frac{dx}{dt}=+\frac{\omega}{k}.
$$

En cambio, $kx+\omega t=\text{constante}$ da $dx/dt=-\omega/k$: la onda avanza hacia $-x$. El signo delante de $\omega t$ indica el sentido; no se debe cambiar sin cambiar la dirección física de propagación.

![[imagenes/sentido-fase-onda.svg]]

## 6. De una frase a los vectores

Antes de escribir $\vec E(x,t)$ y $\vec B(x,t)$:

1. Dibuja los ejes y señala el sentido de avance $\hat n$.
2. Escribe el sentido del campo eléctrico.
3. Calcula el sentido de $\vec B$ con $\hat n\times\vec E$.
4. Elige la fase que viaja en el sentido indicado.
5. Comprueba al final que $\vec E\times\vec B$ apunta como $\hat n$.

La elección de orientación de $\vec E$ puede ser arbitraria si el problema no la fija, pero una vez elegida, la orientación de $\vec B$ debe ser compatible. Si el enunciado solo da magnitudes, declara la convención de ejes elegida: así las ecuaciones vectoriales quedan inequívocas.

## Errores que conviene evitar

- Confundir la dirección en que oscila un campo con la dirección en que avanza la onda.
- Usar $E_{max}=cB_{max}$ sin convertir militeslas a teslas.
- Poner $kx-\omega t$ para una onda que viaja en $-x$.
- Elegir la dirección de $\vec B$ solo por inspección; comprueba el producto vectorial.
- Olvidar que $k$ tiene unidades de $\mathrm{rad/m}$ y $\omega$ de $\mathrm{rad/s}$.

## Fuentes de esta nota

La presentación de Ondas Electromagnéticas explica la interacción de los campos y la propagación sin medio (Zotero, pp. 2–5). La práctica de ondas electromagnéticas aporta el problema del láser usado como transferencia (Zotero, p. 2). Véase [[Fuentes Zotero y probabilidad]].
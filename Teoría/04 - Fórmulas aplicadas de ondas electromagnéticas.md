---
tags: [fisica-aplicada, teoria, formulas, ondas-em]
---

# Fórmulas aplicadas — ondas electromagnéticas

[[Teoría/04 - Ondas electromagnéticas|← Índice del módulo]] · [[Teoría/04 - Conceptos de ondas electromagnéticas|Conceptos]]

## Magnitudes y unidades

| Símbolo | Significado | Unidad SI |
|---|---|---|
| $\lambda$ | Longitud de onda | $\mathrm m$ |
| $f$ | Frecuencia | $\mathrm{Hz}=\mathrm{s^{-1}}$ |
| $T$ | Período | $\mathrm s$ |
| $c$ | Rapidez de propagación en el vacío | $\mathrm{m/s}$ |
| $k$ | Número de onda | $\mathrm{rad/m}$ |
| $\omega$ | Frecuencia angular | $\mathrm{rad/s}$ |
| $E_{max}$ | Amplitud del campo eléctrico | $\mathrm{V/m}$ |
| $B_{max}$ | Amplitud del campo magnético | $\mathrm T$ |

Convierte primero: $1\,\mathrm{nm}=10^{-9}\,\mathrm m$, $1\,\mathrm{\mu m}=10^{-6}\,\mathrm m$, $1\,\mathrm{mT}=10^{-3}\,\mathrm T$ y $1\,\mathrm{MV/m}=10^6\,\mathrm{V/m}$.

## 1. Rapidez, frecuencia y longitud de onda

$$
c=\lambda f,\qquad
f=\frac{c}{\lambda},\qquad
\lambda=\frac{c}{f}.
$$

**Cuándo usarla:** cuando el enunciado da la longitud de onda o la frecuencia de una onda en el vacío. La rapidez $c$ es fija en este módulo. Un ciclo ocupa una distancia $\lambda$ y tarda un período $T=1/f$, así que la rapidez es $v=\lambda/T=\lambda f=c$.

## 2. Número de onda y frecuencia angular

Un ciclo completo cambia la fase en $2\pi$ radianes. Por eso, al dividir ese cambio por el tamaño espacial o temporal de un ciclo:

$$
k=\frac{2\pi}{\lambda},\qquad
\omega=2\pi f,\qquad
\omega=ck.
$$

Usa $k$ en la fase espacial y $\omega$ en la fase temporal. La relación $\omega=ck$ es una comprobación equivalente de que se está describiendo una onda en el vacío.

## 3. Relación entre amplitudes

Para una onda plana sinusoidal en el vacío, las ecuaciones de Maxwell relacionan los máximos de ambos campos:

$$
E_{max}=cB_{max},\qquad
B_{max}=\frac{E_{max}}{c}.
$$

Elige la forma que despeja directamente la incógnita. La comprobación dimensional es útil: $(\mathrm{m/s})(\mathrm T)=\mathrm{V/m}$.

**De dónde sale:** en una onda plana, las leyes de Faraday y Ampère-Maxwell relacionan las variaciones espaciales y temporales de ambos campos. Para campos sinusoidales en fase, al comparar sus derivadas se obtiene $kE_{max}=\omega B_{max}$. Como $\omega/k$ es la rapidez de la onda y en el vacío vale $c$, resulta $E_{max}/B_{max}=c$.

## 4. Dirección de los campos

Sea $\hat n$ el vector unitario de propagación. La orientación del campo magnético queda determinada por

$$
\vec B=\frac{1}{c}\,\hat n\times\vec E,
\qquad
\vec E\times\vec B\ \text{apunta en la dirección de}\ \hat n.
$$

Para decidir el sentido, trabaja con unitarios cartesianos: $\hat x\times\hat y=\hat z$, $\hat y\times\hat z=\hat x$ y $\hat z\times\hat x=\hat y$. Invertir el orden invierte el signo.

## 5. Ecuaciones de campo y sentido de viaje

En el eje $x$, las formas sinusoidales usuales son

$$
\vec E(x,t)=\vec E_{max}\cos(kx-\omega t+\phi_0),
\qquad
\vec B(x,t)=\vec B_{max}\cos(kx-\omega t+\phi_0)
$$

para propagación en $+x$. Para propagación en $-x$, cambia la fase a $kx+\omega t+\phi_0$. Los vectores amplitud $\vec E_{max}$ y $\vec B_{max}$ contienen tanto la magnitud como la dirección; deben respetar la regla del producto vectorial. Ambos campos comparten la misma fase.

Una forma que sirve para cualquier dirección es

$$
\vec E(\vec r,t)=\vec E_{max}\cos(\vec k\cdot\vec r-\omega t+\phi_0),
$$

con $\vec k=k\hat n$. El parcial puede resolverse en una dimensión usando $x$ y el signo de la fase.

## Receta de resolución

1. Dibuja los ejes y escribe la dirección de propagación.
2. Convierte todos los datos a SI.
3. Calcula $f=c/\lambda$ o $\lambda=c/f$.
4. Calcula la amplitud que falta con $E_{max}=cB_{max}$.
5. Calcula $k=2\pi/\lambda$ y $\omega=2\pi f$.
6. Elige el signo de la fase a partir del sentido de viaje.
7. Obtén la dirección del otro campo con $\hat n\times\vec E$.
8. Escribe las dos ecuaciones y comprueba $\vec E\times\vec B$.

## Controles rápidos

- $E_{max}/B_{max}$ debe dar $3.00\times10^8\,\mathrm{m/s}$.
- Si la onda avanza en $-x$, la fase unidimensional debe tener $+\omega t$.
- Los tres sentidos deben ser mutuamente perpendiculares.
- Si usas amplitudes positivas junto con unitarios, el signo va en el unitario, no escondido en la fase.
- Un valor en $\mathrm{mT}$ o $\mathrm{nm}$ debe convertirse antes de calcular.
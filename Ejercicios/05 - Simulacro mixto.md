---
tags: [fisica-aplicada, simulacro, parcial]
---

# Simulacro mixto del segundo parcial

**Duración:** 90 minutos · **Puntaje:** 100 puntos · **Modalidad:** sin apuntes durante el intento.

Este simulacro mezcla las cuatro familias confirmadas para el parcial. Distribuye unos 20 minutos por problema y deja 10 minutos para revisar unidades, signos y respuestas. Escribe el modelo físico antes de sustituir números; un resultado sin justificación pierde parte del puntaje.

**Constantes:** $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$; $c=3.00\times10^8\,\mathrm{m/s}$; $I_0=1.00\times10^{-12}\,\mathrm{W/m^2}$; rapidez del sonido $v=343\,\mathrm{m/s}$.

> [!info] Cómo rendirlo
> En cada problema anota: datos y unidades SI, dibujo o convención de signos, principio físico, ecuación antes de reemplazar, cálculo y control final. No abras [[Resoluciones/05 - Simulacro mixto]] hasta terminar los cuatro.

## Problema 1 — Campo gravitatorio por superposición · 25 puntos · 20 min

Dos masas puntuales fijas producen un campo gravitatorio en el origen $O$. Una masa de prueba de $150\,\mathrm{kg}$ se coloca en ese punto.

**Datos**

- $M_1=4.00\times10^{11}\,\mathrm{kg}$ en $A=(-3.00,0)\,\mathrm{km}$.
- $M_2=9.00\times10^{11}\,\mathrm{kg}$ en $B=(0,4.00)\,\mathrm{km}$.
- $O=(0,0)$.

![[imagenes/campo-no-simetrico.svg]]

**Se pide**

1. Convierte las posiciones a metros y determina la dirección del campo que produce cada masa en $O$.
2. Calcula las componentes $g_x$ y $g_y$, el módulo $|\vec g|$ y su dirección, expresada como ángulo **al norte del oeste**.
3. Calcula la fuerza gravitatoria vectorial sobre la masa de prueba y explica por qué el campo no depende de esa masa.

> [!tip]- Pista plegable
> Calcula por separado $GM_1/r_1^2$ y $GM_2/r_2^2$. Asigna los signos con el dibujo antes de sumar; la fuerza sobre la masa de prueba se obtiene mediante $\vec F=m\vec g$.

## Problema 2 — Tiempo propio y longitud propia · 25 puntos · 20 min

Una nave se mueve con rapidez constante $0.800c$ respecto de la Tierra.

- Dos destellos emitidos desde un mismo punto de la nave están separados por un intervalo propio de $4.00\,\mathrm{años}$, medido por un reloj que viaja con la nave.
- La longitud propia de la nave, medida en reposo respecto de ella, es $180\,\mathrm{m}$.

**Se pide**

1. Calcula el factor de Lorentz $\gamma$.
2. Determina cuánto tiempo separa esos eventos según la Tierra. Indica cuál de los dos intervalos es propio y por qué.
3. Calcula la longitud que mide la Tierra y explica qué condición de simultaneidad debe cumplir esa medición.

> [!tip]- Pista plegable
> Para el intervalo temporal, identifica el marco donde ambos eventos ocurren en el mismo lugar. Para la longitud, identifica el marco donde la nave está en movimiento y los extremos se registran simultáneamente.

## Problema 3 — Nivel sonoro y efecto Doppler · 25 puntos · 25 min

### a. Dos fuentes independientes · 12 puntos

Una máquina produce en el puesto de medición un nivel sonoro de $72.0\,\mathrm{dB}$. Se enciende una segunda máquina idéntica e independiente; ambas aportan la misma intensidad en el puesto.

Calcula la intensidad de una máquina, la intensidad total y el nuevo nivel sonoro. Explica por qué no se duplican los decibeles.

### b. Fuente y observador que se acercan · 13 puntos

Una sirena emite una frecuencia de $600\,\mathrm{Hz}$. La fuente se acerca a un observador a $25.0\,\mathrm{m/s}$ y el observador se acerca a la fuente a $10.0\,\mathrm{m/s}$. El aire está en reposo respecto del suelo.

Calcula la frecuencia que recibe el observador. Antes de usar la ecuación de Doppler, indica qué efecto tiene cada movimiento sobre la frecuencia.

> [!tip]- Pista plegable
> En el primer apartado suma intensidades antes de usar el logaritmo. En el segundo, ambos movimientos son de acercamiento: la fuente comprime los frentes por delante y el observador los encuentra más rápido.

## Problema 4 — Onda electromagnética en el vacío · 25 puntos · 25 min

Una onda electromagnética sinusoidal se propaga en el vacío hacia $+z$. Su longitud de onda es $20.0\,\mathrm{\mu m}$ y su campo magnético máximo vale $1.80\,\mathrm{mT}$. En $z=0$ y $t=0$, el campo eléctrico apunta hacia $+x$ y alcanza su máximo positivo.

**Se pide**

1. Convierte los datos a SI y calcula $f$, $E_{\max}$, $k$ y $\omega$.
2. Determina la dirección de $\vec B_{\max}$ usando el producto vectorial.
3. Escribe $\vec E(z,t)$ y $\vec B(z,t)$.
4. Comprueba que la fase describe propagación hacia $+z$ y que $\vec E\times\vec B$ apunta en el mismo sentido.

> [!tip]- Pista plegable
> Usa $f=c/\lambda$, $E_{\max}=cB_{\max}$, $k=2\pi/\lambda$ y $\omega=2\pi f$. Para la dirección, aplica $\hat n\times\vec E_{\max}$; para una onda que avanza en $+z$, prueba la fase $kz-\omega t$.

## Entrega y autocorrección

Antes de consultar las soluciones, revisa:

- ¿Convertí todas las distancias, frecuencias y amplitudes a unidades compatibles?
- ¿Justifiqué por qué se aplica cada modelo?
- ¿Conservé los sentidos vectoriales y las convenciones de signos?
- ¿El orden de magnitud y la unidad del resultado tienen sentido?

Después compara con [[Resoluciones/05 - Simulacro mixto]] y anota cada error en [[Ejercicios/00 - Método y registro]].

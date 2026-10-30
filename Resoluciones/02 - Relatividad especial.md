---
tags: [fisica-aplicada, resoluciones, relatividad]
---

# Resoluciones modelo — Relatividad especial

**Ejercicios:** [[Ejercicios/02 - Relatividad especial]] · **Conceptos:** [[Teoría/02 - Conceptos de relatividad especial]] · **Fórmulas justificadas:** [[Teoría/02 - Fórmulas aplicadas de relatividad especial]]

Lee cada resolución con lápiz y papel: pausa antes del despeje, predice el siguiente paso y explica por qué aplica esa ley. Los cálculos conservan la convención de signos de la hoja de fórmulas.

## Rutina que se repite

1. Describe qué se mide y cuáles son los eventos o cuerpos.
2. Indica el marco que mide cada dato.
3. Selecciona el principio físico y explica por qué aplica.
4. Plantea primero con símbolos; despeja antes de sustituir.
5. Sustituye con unidades, calcula y controla el resultado.

---

## 8. Dilatación temporal: tiempo propio conocido

**Interpretación.** La tripulación mide el intervalo entre dos eventos que ocurren en el mismo lugar de la nave. Por tanto, su reloj mide el tiempo propio $\Delta t_0$. La Tierra observa ese reloj en movimiento y mide el intervalo dilatado $\Delta t$.

**Datos e incógnita**

$$
v=0.60c,\qquad \Delta t_0=1.00\,\mathrm{h},\qquad
\text{incógnita: }\Delta t.
$$

**Principio.** Para los mismos eventos, el tiempo medido desde el marco donde el reloj se mueve es $\Delta t=\gamma\Delta t_0$. La fórmula es adecuada porque los eventos ocurren en el mismo lugar de la nave, lo que permite identificar el tiempo propio.

**Cálculo**

$$
\gamma=\frac{1}{\sqrt{1-(0.60)^2}}
=\frac{1}{0.80}=1.25,
$$

$$
\Delta t=(1.25)(1.00\,\mathrm{h})=1.25\,\mathrm{h}.
$$

**Resultado y control.** La Tierra mide $1.25\,\mathrm{h}=1\,\mathrm{h}\,15\,\mathrm{min}$. Es mayor que el tiempo propio, como exige la dilatación temporal.

---

## 9. Dilatación temporal: hallar el tiempo propio

**Interpretación.** La Tierra mide $\Delta t=5.00\,\mathrm{h}$; la nave y su reloj se mueven a $0.80c$. Se busca el intervalo propio de la nave.

**Datos e incógnita**

$$
v=0.80c,\qquad \Delta t=5.00\,\mathrm{h},\qquad
\text{incógnita: }\Delta t_0.
$$

**Principio.** Se usa $\Delta t=\gamma\Delta t_0$ porque se comparan los mismos dos eventos y la nave mide el intervalo en el marco donde su reloj está en reposo.

**Despeje y cálculo**

$$
\gamma=\frac{1}{\sqrt{1-(0.80)^2}}
=\frac{1}{0.60}=1.6667,
$$

$$
\Delta t_0=\frac{\Delta t}{\gamma}
=\frac{5.00\,\mathrm{h}}{1.6667}
=3.00\,\mathrm{h}.
$$

**Resultado y control.** El reloj de la nave registra $3.00\,\mathrm{h}$; es menor que las $5.00\,\mathrm{h}$ terrestres. Si resultara mayor, se habría invertido el despeje.

---

## 10. Rapidez para que los relojes difieran un 1 %

**Interpretación.** El enunciado define que el intervalo exterior es 1 % mayor que el tiempo propio. Es decir, $\Delta t=1.01\Delta t_0$. Esto evita confundir “un 1 % de diferencia” con una razón invertida.

**Paso 1: identificar $\gamma$**

$$
\gamma=\frac{\Delta t}{\Delta t_0}=1.01.
$$

**Paso 2: despejar la rapidez**

Partimos de $\gamma=1/\sqrt{1-v^2/c^2}$. Elevamos al cuadrado, invertimos y despejamos:

$$
\frac{1}{\gamma^2}=1-\frac{v^2}{c^2},
\qquad
\frac{v}{c}=\sqrt{1-\frac{1}{\gamma^2}}.
$$

**Paso 3: sustituir**

$$
\frac{v}{c}
=\sqrt{1-\frac{1}{(1.01)^2}}
=0.1404.
$$

**Resultado y control.** La rapidez es $v\approx0.140c$. En unidades SI,

$$
v=(0.1404)(3.00\times10^8\,\mathrm{m/s})
=4.21\times10^7\,\mathrm{m/s}.
$$

La rapidez es menor que $c$ y produce $\gamma=1.01$, consistente con la diferencia temporal indicada. Este tipo aparece en el modelo 2024 y su resolución guardada en Zotero.

---

## 11. Contracción de longitud de una nave

**Interpretación.** La longitud dada es la propia $L_0$ porque la tripulación la mide en reposo respecto de la nave. La Tierra mide la nave en movimiento y pide su longitud paralela al movimiento.

**Datos e incógnita**

$$
v=0.87c,\qquad L_0=350\,\mathrm{m},\qquad
\text{incógnita: }L.
$$

**Principio.** Se usa $L=L_0/\gamma$. La longitud terrestre se obtiene midiendo las posiciones de los dos extremos simultáneamente en el marco terrestre; solo la dimensión paralela al movimiento se contrae.

**Cálculo**

$$
\gamma=\frac{1}{\sqrt{1-(0.87)^2}}
=\frac{1}{\sqrt{0.2431}}
\approx2.028,
$$

$$
L=\frac{350\,\mathrm{m}}{2.028}
\approx172.6\,\mathrm{m}.
$$

**Resultado y control.** La Tierra mide aproximadamente $173\,\mathrm{m}$. Es menor que $L_0=350\,\mathrm{m}$; la longitud propia debe ser la mayor. Para visualizar qué significa medir los dos extremos al mismo tiempo, consulta ![[imagenes/medicion-longitud-simultanea.svg]].

Este es el tipo de contracción incluido en el modelo DOCX 2025 de Zotero.

---

## 12. Suma relativista de velocidades y tiempo de llegada

![[imagenes/marcos-relatividad.svg]]

**Interpretación y eje.** Usamos el marco terrestre $S$ y elegimos $+x$ hacia la Tierra. La nave se mueve en $+x$ a $v=0.400c$. El proyectil también avanza en $+x$ respecto de la nave a $u'=0.700c$. Buscamos su velocidad $u$ respecto de la Tierra.

**Principio.** Las velocidades se miden en marcos distintos y son relativistas. Se aplica la transformación colineal $u=(u'+v)/(1+u'v/c^2)$, que conserva $c$ como límite.

**Paso 1: sumar las velocidades relativísticamente**

$$
u=\frac{0.700c+0.400c}{1+(0.700)(0.400)}
=\frac{1.100}{1.280}c
=0.859375c.
$$

La rapidez terrestre del proyectil es $u\approx0.8594c$.

**Paso 2: reunir distancia y velocidad en el mismo marco**

La distancia inicial $D=8.00\times10^6\,\mathrm{km}$ y $u$ corresponden al marco terrestre. Convertimos:

$$
D=(8.00\times10^6\,\mathrm{km})
(10^3\,\mathrm{m/km})
=8.00\times10^9\,\mathrm{m},
$$

$$
u=(0.859375)(3.00\times10^8\,\mathrm{m/s})
=2.578\times10^8\,\mathrm{m/s}.
$$

**Paso 3: calcular el tiempo terrestre de llegada**

$$
t=\frac{D}{u}
=\frac{8.00\times10^9\,\mathrm{m}}
{2.578\times10^8\,\mathrm{m/s}}
=31.0\,\mathrm{s}.
$$

**Resultado y control.** La Tierra mide $u=+0.8594c$ y un tiempo de llegada de aproximadamente $31.0\,\mathrm{s}$. No se suma para obtener $1.10c$: el resultado relativista es menor que $c$. La distancia y velocidad usadas en $t=D/u$ pertenecen ambas al marco terrestre.

El enunciado y el método corresponden al problema de velocidades relativistas de la práctica guardada en Zotero y al tipo del modelo PDF 2025.

---

## 13. Suma relativista en sentidos opuestos

**Interpretación y signos.** Tomamos $+x$ hacia el movimiento de la nave. En la Tierra, la nave tiene $v=+0.80c$. En la nave, el proyectil se dispara hacia atrás, de modo que $u'=-0.60c$. El signo negativo es información física: no debe reemplazarse por el módulo.

**Principio y ecuación.** Como se transforma una velocidad colineal entre dos marcos, usamos

$$
u=\frac{u'+v}{1+u'v/c^2}.
$$

**Cálculo**

$$
u=\frac{-0.60c+0.80c}{1+(-0.60)(0.80)}
=\frac{0.20}{0.52}c
=+0.3846c.
$$

**Resultado y control.** En el marco terrestre el proyectil sigue avanzando en $+x$, a $0.3846c$. Aunque fue disparado hacia atrás respecto de la nave, la nave se mueve más rápido que ese retroceso. El módulo final es menor que $c$ y el signo positivo confirma el sentido.

## Fuentes cotejadas

- [Capítulo de relatividad](zotero://select/library/items/YB8669CS), PDF pp. 7–9, 12–15 y 17–19.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), PDF p. 25: velocidades $0.400c$ y $0.700c$ y tiempo de alcance.
- [Modelo PDF 2025, escaneado](zotero://select/library/items/6GRRT3TK), p. 2: suma relativista seguida del tiempo de alcance; página revisada como imagen.
- [Modelo DOCX 2025](zotero://select/library/items/DHM5X7QD): contracción de longitud a $0.87c$.
- [Resolución del modelo 2024](zotero://select/library/items/UHEXA2AW): diferencia temporal del 1 %.

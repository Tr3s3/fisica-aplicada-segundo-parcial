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

## C1. Identificar el tiempo propio en dos marcos

**Interpretación de los eventos.** En los dos incisos comparamos A, cuando Magda pasa junto a Sergio, con B, cuando Magda alcanza el punto final señalado. En el marco terrestre, la nave se desplaza entre A y B. En el marco de Magda, ambos eventos ocurren en el mismo lugar de la nave; por eso el cronómetro de Magda mide el tiempo propio $\Delta t_0$.

**Datos e incógnitas**

$$
v=0.600c,\qquad \Delta x_{S}=9.00\times10^7\,\mathrm{m},\qquad c=3.00\times10^8\,\mathrm{m/s}.
$$

### (a) Partir de la distancia medida por Sergio

**Paso 1: hallar el intervalo terrestre.** La distancia y la rapidez están medidas respecto de la Tierra. Por eso Sergio calcula

$$
\Delta t_S=\frac{\Delta x_S}{v}
=\frac{9.00\times10^7\,\mathrm{m}}{0.600(3.00\times10^8\,\mathrm{m/s})}
=0.500\,\mathrm{s}.
$$

**Paso 2: calcular el factor de Lorentz.**

$$
\gamma=\frac{1}{\sqrt{1-(0.600)^2}}=1.25.
$$

**Paso 3: hallar el intervalo propio de Magda.** Sergio ve el reloj de Magda en movimiento, así que mide el intervalo dilatado $\Delta t_S=\gamma\Delta t_0$:

$$
\Delta t_0=\frac{\Delta t_S}{\gamma}
=\frac{0.500\,\mathrm{s}}{1.25}
=0.400\,\mathrm{s}.
$$

**Resultado y control.** Sergio mide $0.500\,\mathrm{s}$ y Magda $0.400\,\mathrm{s}$. El tiempo propio es menor. El criterio es que ambos eventos ocurran en el mismo lugar del marco de Magda, no que su cronómetro marque el mayor valor.

### (b) Comprobar desde el tiempo propio

Si el cronómetro de Magda registra $\Delta t_0=0.400\,\mathrm{s}$, Sergio registra

$$
\Delta t_S=\gamma\Delta t_0=(1.25)(0.400\,\mathrm{s})=0.500\,\mathrm{s}.
$$

Se recupera el mismo intervalo terrestre que en (a). Este segundo cálculo confirma que ambas partes describen el mismo par de eventos.

## C2. Separación de dos observadores vista desde una nave

**Interpretación.** Los dos observadores están fijos en la Tierra, así que su separación se mide en el marco donde el par está en reposo. Esa es la longitud propia $L_0$. La nave se mueve paralela a la línea entre ellos; la tripulación mide esa separación como una longitud contraída.

**Datos e incógnita**

$$
L_0=56.4\,\mathrm{m},\qquad v=0.990c,\qquad \text{incógnita: }L_{\text{nave}}.
$$

**Principio.** Usamos $L=L_0\sqrt{1-v^2/c^2}$ porque la separación es paralela al movimiento relativo.

**Cálculo**

$$
L_{\text{nave}}=(56.4\,\mathrm{m})\sqrt{1-(0.990)^2}
=(56.4\,\mathrm{m})\sqrt{0.0199}
=7.95\,\mathrm{m}.
$$

**Resultado y control.** La tripulación mide aproximadamente $7.95\,\mathrm{m}$ entre los observadores. Es menor que los $56.4\,\mathrm{m}$ medidos en el marco donde ellos están en reposo. Cada observador debe medir las dos posiciones simultáneamente en su propio marco; las dos respuestas no son dos lecturas de una misma pareja de eventos simultáneos.

## C3. Hallar la rapidez a partir de una longitud contraída

**Interpretación.** La regla mide $L_0=1.00\,\mathrm{m}$ en su propio marco y se mueve paralela a su eje. La observadora mide $L=0.3048\,\mathrm{m}$. Como conoce ambas longitudes, despejamos la rapidez de la fórmula de contracción.

**Despeje**

$$
L=L_0\sqrt{1-\frac{v^2}{c^2}}
\quad\Longrightarrow\quad
\frac{v}{c}=\sqrt{1-\left(\frac{L}{L_0}\right)^2}.
$$

**Cálculo**

$$
\frac{v}{c}=\sqrt{1-\left(\frac{0.3048\,\mathrm{m}}{1.00\,\mathrm{m}}\right)^2}
=0.9524,
$$

$$
v=(0.9524)(3.00\times10^8\,\mathrm{m/s})
=2.86\times10^8\,\mathrm{m/s}.
$$

**Resultado y control.** La regla se mueve a $v\approx0.952c$. La rapidez es menor que $c$, y que $L/L_0\approx0.305$ corresponde a una contracción fuerte, como cabe esperar a esta rapidez.

## C4. Longitud de una pista y tiempos medidos en dos marcos

![[imagenes/medicion-longitud-simultanea.svg]]

**Marcos y eventos.** La pista está en reposo en la Tierra, por lo que $L_0=3600\,\mathrm{m}$ es su longitud propia. Los eventos son el paso de la nave por cada extremo. Para el piloto ocurren en el mismo lugar de la nave, así que su intervalo es el tiempo propio $\Delta t_0$.

**Datos**

$$
L_0=3600\,\mathrm{m},\qquad v=4.00\times10^7\,\mathrm{m/s},\qquad c=3.00\times10^8\,\mathrm{m/s}.
$$

### (a) Longitud de la pista en el marco de la nave

La rapidez relativa como fracción de $c$ es $\beta=v/c=0.1333$. La pista se mueve en el marco del piloto, así que

$$
L=L_0\sqrt{1-\beta^2}
=(3600\,\mathrm{m})\sqrt{1-(0.1333)^2}
=3568\,\mathrm{m}.
$$

### (b) Tiempo medido desde la Tierra

La nave recorre los $3600\,\mathrm{m}$ de la pista en el marco terrestre:

$$
\Delta t=\frac{L_0}{v}
=\frac{3600\,\mathrm{m}}{4.00\times10^7\,\mathrm{m/s}}
=9.00\times10^{-5}\,\mathrm{s}.
$$

### (c) Tiempo medido por el piloto

En el marco de la nave, la pista contraída pasa frente al piloto. Usamos esa longitud y la rapidez relativa en el mismo marco:

$$
\Delta t_0=\frac{L}{v}
=\frac{3568\,\mathrm{m}}{4.00\times10^7\,\mathrm{m/s}}
=8.92\times10^{-5}\,\mathrm{s}.
$$

**Comprobación.** $\gamma=1/\sqrt{1-\beta^2}=1.009$. Entonces

$$
\gamma\Delta t_0=(1.009)(8.92\times10^{-5}\,\mathrm{s})
\approx9.00\times10^{-5}\,\mathrm{s}=\Delta t.
$$

Los resultados concuerdan: el tiempo terrestre es mayor que el tiempo propio del piloto. La comprobación solo funciona porque cada distancia y rapidez usadas en $\Delta t=d/v$ pertenecen al mismo marco.

## C5. Energía y rapidez de electrones

> [!note] Alcance
> Este ejercicio extiende la práctica a energía relativista porque aparece en el TP, pero no en los modelos de parcial revisados. Déjalo para después de los tipos de prioridad alta.

**Principio físico.** La energía en reposo del electrón es $E_0=m_ec^2$. Al acelerarlo desde el reposo mediante una diferencia de potencial, el campo eléctrico realiza un trabajo de magnitud $K=e|\Delta V|$. La energía total pasa a ser $E=E_0+K=\gamma m_ec^2$; por tanto, $\gamma=1+K/E_0$ y $v/c=\sqrt{1-1/\gamma^2}$.

### (a) Energía en reposo

$$
E_0=m_ec^2
=(9.11\times10^{-31}\,\mathrm{kg})(2.998\times10^8\,\mathrm{m/s})^2
=8.19\times10^{-14}\,\mathrm{J}.
$$

Para convertir a electronvoltios usamos $1\,\mathrm{eV}=1.602\times10^{-19}\,\mathrm{J}$:

$$
E_0=\frac{8.19\times10^{-14}\,\mathrm{J}}{1.602\times10^{-19}\,\mathrm{J/eV}}
=5.11\times10^5\,\mathrm{eV}=0.511\,\mathrm{MeV}.
$$

Usamos $c=2.998\times10^8\,\mathrm{m/s}$ en este cálculo para conservar la precisión de la energía en reposo.

### (b) Rapidez final

**Para $20.0\,\mathrm{kV}$.** La energía cinética ganada es $K=e\Delta V=20.0\,\mathrm{keV}=0.0200\,\mathrm{MeV}$:

$$
\gamma=1+\frac{0.0200}{0.511}=1.039,
\qquad
\frac{v}{c}=\sqrt{1-\frac{1}{(1.039)^2}}=0.272,
$$

$$
v=(0.272)(2.998\times10^8\,\mathrm{m/s})
=8.15\times10^7\,\mathrm{m/s}.
$$

**Para $5.00\,\mathrm{MV}$.** Ahora $K=e\Delta V=5.00\,\mathrm{MeV}$:

$$
\gamma=1+\frac{5.00}{0.511}=10.78,
\qquad
\frac{v}{c}=\sqrt{1-\frac{1}{(10.78)^2}}=0.9957,
$$

$$
v=(0.9957)(2.998\times10^8\,\mathrm{m/s})
=2.99\times10^8\,\mathrm{m/s}.
$$

**Control.** Al aumentar la diferencia de potencial, aumenta $\gamma$ y la rapidez se acerca a $c$, pero no la alcanza. La energía cinética adicional de $5.00\,\mathrm{MeV}$ es mucho mayor que la energía en reposo del electrón, por eso el segundo resultado queda muy próximo a $c$.

## Fuentes cotejadas

- [Capítulo de relatividad](zotero://select/library/items/YB8669CS), PDF pp. 7–9, 12–15 y 17–19.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), PDF pp. 13–24: intervalos propios, contracción, pista espacial y energía de electrones para los complementarios C1–C5.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), PDF p. 25: velocidades $0.400c$ y $0.700c$ y tiempo de alcance.
- [Modelo PDF 2025, escaneado](zotero://select/library/items/6GRRT3TK), p. 2: suma relativista seguida del tiempo de alcance; página revisada como imagen.
- [Modelo DOCX 2025](zotero://select/library/items/DHM5X7QD): contracción de longitud a $0.87c$.
- [Resolución del modelo 2024](zotero://select/library/items/UHEXA2AW): diferencia temporal del 1 %.

---
tags: [fisica-aplicada, teoria, gravitacion, formulas]
---

# Fórmulas aplicadas — Gravitación y órbitas

**Recorrido:** [[Teoría/01 - Gravitación y órbitas|Índice]] · [[Teoría/01 - Conceptos de gravitación y órbitas|Conceptos]] · [[Ejercicios/01 - Gravitación y órbitas|Práctica]] · [[Resoluciones/01 - Gravitación y órbitas|Resoluciones]]

## Antes de calcular

- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$, salvo que se indique otro valor.
- Convierte longitudes a metros, masas a kilogramos y períodos a segundos.
- Si dan **altura** $h$, calcula $r=R+h$. Si dan radio orbital $5R$, ese ya es $r$.
- Define ejes y sentidos antes de sumar campos.
- Modela una fuente como masa puntual o como esfera simétrica vista desde fuera; no uses estas expresiones interiores sin otro modelo.
- En rapidez y período orbitales, la masa del satélite se cancela. En energía total sí aparece, así que verifica el dato de masa del satélite.
- En los ejercicios de este módulo, el cuerpo central domina la atracción y se ignoran otras fuerzas salvo que el enunciado diga lo contrario.

> [!abstract] Mapa rápido
> - Fuerza entre masas: ley de gravitación.
> - Campo en un punto: calcula $GM/r^2$ para cada fuente y suma vectores.
> - Peso entre superficie y altura: razón de cuadrados.
> - Peso aparente en un ecuador que rota: gravedad menos aceleración centrípeta.
> - Rapidez o período circular: gravedad proporciona aceleración centrípeta.
> - Energía orbital o escape: conservación de energía.
> - Comparación de órbitas: tercera ley de Kepler.
> - Masa central con $T,r$: despeja la tercera ley.

## 1. Fuerza y campo

$$
F_g=G\frac{Mm}{r^2}.
$$

$M,m$ son masas; $r$, la separación entre centros. La fuerza apunta hacia la otra masa.

El campo se obtiene dividiendo la fuerza por la masa de prueba:

$$
g=\frac{F_g}{m}=G\frac{M}{r^2}.
$$

La masa de prueba se cancela. Usa esta relación cuando pidan campo o aceleración gravitatoria.

Para sumar fuentes, proyecta sus campos en ejes y conserva signos:

$$
g_x=\sum_i g_i\cos\theta_i,\qquad
g_y=\sum_i g_i\sin\theta_i.
$$

Con coordenadas, una forma vectorial directa es

$$
\vec g(P)=\sum_i GM_i
\frac{\vec r_i-\vec r_P}{|\vec r_i-\vec r_P|^3},
$$

donde $\vec r_i$ ubica la fuente y $\vec r_P$ el punto de cálculo. El numerador apunta desde el punto hacia la masa.

Luego,

$$
|\vec g|=\sqrt{g_x^2+g_y^2}.
$$

Interpreta los signos para ubicar el cuadrante. “Al norte del oeste” significa medir desde el oeste hacia el norte:

$$
\theta=\tan^{-1}\left(\frac{|g_y|}{|g_x|}\right).
$$

Peso y fuerza sobre una masa:

$$
\vec F_g=m\vec g,\qquad W=mg.
$$

## 2. Campo y peso a una altura

Para radio planetario $R$ y altura $h$,

$$
r=R+h,\qquad
g(h)=\frac{GM}{(R+h)^2}.
$$

En superficie $g_0=GM/R^2$. Al dividir las dos expresiones, se cancela $GM$:

$$
\frac{g(h)}{g_0}=\left(\frac{R}{R+h}\right)^2.
$$

Para el mismo objeto $W=mg$, entonces

$$
W_h=W_0\left(\frac{R}{R+h}\right)^2,
\qquad
W_0=W_h\left(\frac{R+h}{R}\right)^2.
$$

Si $h=0.35R$, $r=1.35R$, no $0.35R$. Al comparar pesos no hace falta hallar la masa.

## 3. Órbita circular y período

La aceleración radial necesaria es $v^2/r$. La gravedad la proporciona:

$$
G\frac{Mm}{r^2}=m\frac{v^2}{r}.
$$

Se cancela la masa del satélite y queda

$$
v_{\mathrm{orb}}=\sqrt{\frac{GM}{r}}.
$$

Una vuelta recorre $2\pi r$, así que

$$
T=\frac{2\pi r}{v_{\mathrm{orb}}}
=2\pi\sqrt{\frac{r^3}{GM}}.
$$

La primera forma sirve cuando ya calculaste la rapidez; la segunda, cuando quieres hallar el período directamente.

## 4. Energía orbital y escape

Tomando $U=0$ en el infinito,

$$
U=-\frac{GMm}{r}.
$$

En órbita circular $v^2=GM/r$, por lo que

$$
K=\frac12mv^2=\frac{GMm}{2r},
\qquad
E=K+U=-\frac{GMm}{2r}.
$$

La energía total es negativa: el objeto está ligado.

Para el escape mínimo, la energía final en el infinito es cero:

$$
\frac12m v_{\mathrm{esc}}^2-\frac{GMm}{r}=0
\quad\Rightarrow\quad
v_{\mathrm{esc}}=\sqrt{\frac{2GM}{r}}.
$$

Es la rapidez total en el caso definido; no es necesariamente el $\Delta v$ de un objeto que ya se mueve.

## 5. Kepler y masa central

Reemplazar $v=2\pi r/T$ en la relación orbital da

$$
T^2=\frac{4\pi^2}{GM}r^3,
\qquad
\frac{T^2}{r^3}=\frac{4\pi^2}{GM}.
$$

Para comparar dos órbitas alrededor del mismo cuerpo:

$$
\frac{T_1^2}{r_1^3}=\frac{T_2^2}{r_2^3},
\qquad
r_2=r_1\left(\frac{T_2}{T_1}\right)^{2/3}.
$$

Tierra y Marte orbitan el mismo Sol; puedes usar $T_T=1\,\mathrm{año}$ y $r_T=1\,\mathrm{UA}$ si $T_M$ está en años.

Para hallar la masa central,

$$
M=\frac{4\pi^2r^3}{GT^2}.
$$

Usa segundos y metros; el resultado SI queda en kilogramos.

## 6. Gravedad efectiva en el ecuador de un planeta que rota

La gravedad newtoniana en la superficie es $g=GM/R^2$. Una persona fija respecto del planeta gira con rapidez angular $\\omega=2\\pi/T$ y necesita aceleración centrípeta hacia el centro:

$$
a_c=\\omega^2R=\\frac{4\\pi^2R}{T^2}.
$$

En el ecuador, tomamos hacia el centro como sentido positivo. La gravedad apunta hacia adentro y la fuerza normal $N$ de la balanza hacia afuera:

$$
mg-N=ma_c
\\quad\\Longrightarrow\\quad
g_{\\text{ef}}=\\frac{N}{m}=\\frac{GM}{R^2}-\\frac{4\\pi^2R}{T^2}.
$$

$g_{\\text{ef}}$ determina el peso aparente que leería una balanza: $W_{\\text{ap}}=mg_{\\text{ef}}$. Si piden el resultado en unidades de la gravedad terrestre, divide por $g_\\oplus=9.80\\,\\mathrm{m/s^2}$. Esta aproximación es para el ecuador y desprecia el achatamiento del planeta y otras fuerzas. Se aplica en el ejercicio 9, variante del TP 5, ejercicio 9.

## Controles de plausibilidad

| Resultado | Control |
|---|---|
| Campo o fuerza | Aumentar la distancia reduce el módulo como $1/r^2$; el campo apunta a la fuente. |
| Peso a mayor altura | Debe ser menor que en superficie si $h>0$. |
| Rapidez orbital | A mayor radio, menor rapidez circular para la misma masa central. |
| Energía de órbita circular | Negativa si $U(\infty)=0$. |
| Escape | $v_{\mathrm{esc}}=\sqrt2\,v_{\mathrm{orb}}$ en el mismo radio circular. |
| Kepler | Mayor período alrededor del mismo cuerpo implica mayor radio. |

## Fuentes y correspondencia

Las ecuaciones de gravitación, peso, energía y órbitas se contrastaron con [el capítulo 12 del libro](zotero://select/library/items/ATATDN6I), en particular las ecuaciones 12.1, 12.3–12.5 y 12.9–12.17 (PDF pp. 2, 6, 9, 12–13 y 16). El formulario del [modelo 2025](zotero://select/library/items/6GRRT3TK) también proporciona las expresiones de fuerza, energía circular, escape y período. La corrección de peso aparente se contrastó con el ejercicio 9 del [TP 5](zotero://select/library/items/F4BGIQ83).

**Sigue con:** [[Ejercicios/01 - Gravitación y órbitas]] · [[Resoluciones/01 - Gravitación y órbitas]]

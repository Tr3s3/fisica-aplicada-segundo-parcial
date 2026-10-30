---
tags: [fisica-aplicada, teoria, gravitacion, conceptos]
---

# Conceptos — Gravitación y órbitas

**Recorrido:** [[Teoría/01 - Gravitación y órbitas|Índice]] · [[Teoría/01 - Fórmulas aplicadas de gravitación y órbitas|Fórmulas]] · [[Ejercicios/01 - Gravitación y órbitas|Práctica]] · [[Resoluciones/01 - Gravitación y órbitas|Resoluciones]]

## Qué debes poder explicar

- Por qué la gravedad es atractiva y cómo varía con la distancia.
- Qué diferencia hay entre fuerza gravitatoria, campo y peso.
- Cómo se suman campos de varias masas.
- Por qué un satélite en órbita está en caída libre.
- De dónde salen rapidez y período orbitales, energías y rapidez de escape.
- Cuándo se puede usar la tercera ley de Kepler.

## Modelo físico y límites de uso

Trabajaremos con la gravitación newtoniana: masas puntuales, velocidades muy inferiores a la de la luz y campos suficientemente débiles para ignorar efectos relativistas. Una esfera con distribución esféricamente simétrica produce, en los puntos exteriores, el mismo campo que una masa puntual situada en su centro. Por eso la distancia de las fórmulas se mide entre centros.

> [!abstract] Supuestos que conviene declarar
> - Si el enunciado dice planeta o luna, toma su masa como fuente central y desprecia otros cuerpos salvo que los nombre.
> - En una órbita circular ideal, el satélite está sometido solo a la gravedad; se desprecia el rozamiento y no hay empujes.
> - La rapidez de escape es el umbral para llegar al infinito con rapidez final nula, sin atmósfera ni aporte posterior de energía.
> - Aquí peso significa fuerza gravitatoria. En un cuerpo que rota, la lectura de una balanza puede ser menor: en el ejercicio de Júpiter se calcula ese peso aparente con la aceleración centrípeta.

## 1. Fuerza, campo y peso

Dos masas se atraen. Para masas puntuales separadas por una distancia $r$,

$$
F_g=G\frac{Mm}{r^2}.
$$

$r$ es la distancia **entre sus centros**. Si duplicas $r$, la fuerza queda en una cuarta parte: depende del inverso del cuadrado. Para una esfera simétrica vista desde el exterior, su gravedad se calcula como si toda la masa estuviera concentrada en el centro.

El **campo gravitatorio** es la fuerza gravitatoria por unidad de masa de prueba. Para una fuente de masa $M$ y una masa de prueba $m_{\text{prueba}}$ a distancia $r$:

$$
g=\frac{F_g}{m_{\text{prueba}}}
=\frac{G M m_{\text{prueba}}/r^2}{m_{\text{prueba}}}
=G\frac{M}{r^2}.
$$

La masa de prueba se cancela: el campo depende de la fuente y del punto, no del objeto que pongas allí. Si solo actúa la gravedad, la aceleración es $\vec a=\vec F_g/m_{\text{prueba}}=\vec g$; por eso el primer ejercicio del parcial puede pedir aceleración aunque la suma se resuelva calculando campos. La unidad de $g$ puede escribirse $\mathrm{N/kg}$ o $\mathrm{m/s^2}$. No confundas $G$, constante universal, con $g$, campo local. Como la gravedad es atractiva, el campo apunta desde el punto hacia la fuente.

La fuerza sobre una masa $m$ es $\vec F_g=m\vec g$. Cerca de un planeta esa fuerza se llama **peso**: $W=mg$. La masa mide inercia y no cambia al mover el objeto; el peso es una fuerza y sí cambia cuando cambia $g$.

## 2. Varias fuentes: sumar flechas

Cada fuente aporta un campo y el total es una suma vectorial:

$$
\vec g_{\text{total}}=\sum_i\vec g_i.
$$

No sumes los módulos si las flechas no tienen la misma dirección. En 2D:

1. Dibuja una flecha hacia cada masa desde el punto donde buscas el campo.
2. Calcula cada módulo con $GM_i/r_i^2$.
3. Descompón en $x,y$, conservando signos.
4. Suma componentes; calcula módulo y dirección al final.

Por simetría, componentes horizontales iguales y opuestas se cancelan y las verticales se suman, como en el ejercicio 1.

![[imagenes/campo-gravitatorio.svg]]

En el ejercicio 2, una fuente está al oeste y otra al norte del origen; sus campos tienen signos diferentes en $x$ y $y$.

![[imagenes/campo-no-simetrico.svg]]

## 3. Altura y radio desde el centro

Las fórmulas usan la distancia entre centros. Si el objeto está a altura $h$ sobre un planeta de radio $R$,

$$
r=R+h.
$$

El campo y el peso disminuyen con la distancia, pero la masa permanece constante. Comparar pesos del mismo objeto permite cancelar su masa y $G$.

### Gravedad y peso aparente en un planeta que rota

La gravedad $g=GM/R^2$ es la atracción por unidad de masa. Una balanza, en cambio, mide la fuerza normal $N$ que ejerce el suelo. En el ecuador de un planeta que rota, la persona necesita aceleración centrípeta hacia el centro; por eso la gravedad debe cubrir tanto esa aceleración como la fuerza hacia afuera de la balanza: $mg-N=ma_c$. La lectura por unidad de masa es $N/m=g-a_c$. Este es el ajuste usado en la variante de Júpiter.

![[imagenes/gravedad-rotacion-jupiter.svg]]

![[imagenes/orbita-satelite.svg]]

## 4. Órbita circular: caída libre curvada

Un satélite no escapa a la gravedad: está cayendo continuamente. Su velocidad tangencial hace que la superficie del planeta se curve alejándose debajo de él. En una órbita circular ideal, la gravedad es la fuerza radial neta que curva su trayectoria y produce la aceleración centrípeta.

“Fuerza centrípeta” nombra el papel de la fuerza neta hacia el centro; no es una fuerza adicional que se suma a la gravedad. En una órbita circular ideal, la segunda ley de Newton en la dirección radial queda

$$
\sum F_r = m a_c,
\qquad
G\frac{Mm}{r^2}=m\frac{v^2}{r}.
$$

La gravedad proporciona toda la aceleración centrípeta. La velocidad es tangente a la órbita y la aceleración apunta al centro; como son perpendiculares, la rapidez no cambia, aunque sí cambia la dirección de la velocidad.

## 5. Energía y escape

Tomando la energía potencial igual a cero en el infinito,

$$
U(r)=-\frac{GMm}{r}.
$$

La razón de esta expresión está en el trabajo de una fuerza que varía con la distancia. Si elegimos $U(\infty)=0$ y positivo el sentido radial hacia afuera, la fuerza es $F_r=-GMm/r^2$ y

$$
U(r)-U(\infty)=-\int_{\infty}^{r}F_r\,dr
=-\frac{GMm}{r}.
$$

El signo negativo indica que el sistema ligado tiene menos energía potencial que una masa infinitamente alejada. Al alejar el cuerpo, la gravedad hace trabajo negativo y $U$ aumenta hacia cero; al acercarlo, hace trabajo positivo y $U$ disminuye. La elección del cero es una referencia: lo que se mide directamente son diferencias de energía potencial.

En una órbita circular, $v^2=GM/r$, así que

$$
E=K+U=\frac12m\frac{GM}{r}-\frac{GMm}{r}
=-\frac{GMm}{2r}<0.
$$

La energía mecánica negativa confirma que el satélite está ligado. Para escapar desde el radio $r$, la energía inicial mínima debe igualar la energía final en el infinito. En el umbral, allí $K_f=0$ y $U_f=0$:

$$
\frac12m v_{\text{esc}}^2-\frac{GMm}{r}=0
\quad\Longrightarrow\quad
v_{\text{esc}}=\sqrt{\frac{2GM}{r}}.
$$

Es la rapidez total requerida en el punto de partida; no es automáticamente el incremento de rapidez de un objeto que ya está en órbita.

> [!warning] Rapidez de escape y cambio de rapidez no son lo mismo
> $v_{\text{esc}}=\sqrt{2GM/r}$ es la rapidez total de escape desde ese radio según la definición usual. Si el objeto ya lleva velocidad orbital, la rapidez adicional necesaria depende de la dirección del impulso. En esta guía se pide rapidez de escape, no el $\Delta v$ de una maniobra.

## 6. Kepler: relación entre período y tamaño de órbita

La tercera ley de Kepler relaciona el período con el tamaño de la órbita. Para una órbita circular, $v=2\pi r/T$ y la relación de rapidez orbital es $v^2=GM/r$. Al sustituir la primera en la segunda se obtiene

$$
T^2=\frac{4\pi^2}{GM}r^3.
$$

Para comparar dos cuerpos que orbitan la misma masa central, la constante $4\pi^2/(GM)$ es común y se cancela. Esto permite hallar la distancia de Marte con la órbita terrestre como referencia. La masa del planeta o satélite que orbita se considera despreciable frente a $M$. En una órbita elíptica se usa el semieje mayor $a$ en lugar de $r$; para una circunferencia, $a=r$.

## Secuencia sugerida

1. Explica de memoria campo, fuerza y peso.
2. Estudia [[Teoría/01 - Fórmulas aplicadas de gravitación y órbitas]].
3. Resuelve [[Ejercicios/01 - Gravitación y órbitas]] sin abrir las pistas.
4. Compara con [[Resoluciones/01 - Gravitación y órbitas]] y registra errores.

## Fuentes consultadas

- [Capítulo 12, Gravitación](zotero://select/library/items/ATATDN6I): ley universal y superposición, PDF pp. 2–5 (libro pp. 384–387); peso y variación con la distancia al centro, PDF pp. 6–8 (pp. 388–390); energía potencial y escape, PDF pp. 8–10 (pp. 390–392); órbitas circulares, período y energía, PDF pp. 12–13 (pp. 394–395); leyes de Kepler, PDF pp. 15–17 (pp. 397–399).
- [TP 5: Gravitación, Física Aplicada 2025](zotero://select/library/items/F4BGIQ83), pp. 1–3: superposición, peso, gravedad superficial, Kepler, rotación, satélites y energía.
- [Modelo del segundo parcial, Tema A, 11/11/2025](zotero://select/library/items/6GRRT3TK), pp. 1–2 escaneadas: aceleración por dos masas, satélite lunar y formulario entregado.

La guía explica y reorganiza esas ideas para estudiar. Las etiquetas **M** y **R** distinguen ejercicios del tipo observado en modelos y variantes de transferencia basadas en el TP; no se presentan las variantes como transcripciones literales.

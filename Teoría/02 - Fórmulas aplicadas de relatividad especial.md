---
tags: [fisica-aplicada, teoria, formulas, relatividad]
---

# Fórmulas aplicadas — Relatividad especial

**Volver al módulo:** [[Teoría/02 - Relatividad especial]] · **Conceptos:** [[Teoría/02 - Conceptos de relatividad especial]] · **Práctica:** [[Ejercicios/02 - Relatividad especial]]

> [!important] Antes de elegir una ecuación
> Indica el marco que mide cada dato y dibuja las direcciones. $\Delta t_0$ y $L_0$ no significan “el dato inicial”: el subíndice 0 identifica una medición propia.

## 1. Factor de Lorentz

$$
\beta=\frac{v}{c},\qquad
\gamma=\frac{1}{\sqrt{1-\beta^2}}
=\frac{1}{\sqrt{1-v^2/c^2}}.
$$

- $v$: módulo de la velocidad relativa pertinente entre los dos marcos.
- $c=3.00\times10^8\,\mathrm{m/s}$: rapidez de la luz en el vacío.
- $\gamma$ no tiene unidades, y debe ser mayor o igual que 1.
- Si se da $v=0.60c$, usa directamente $\beta=0.60$.

## 2. Dilatación temporal

Para **los mismos dos eventos**, si ocurren en el mismo punto en un marco:

$$
\Delta t_0=\text{tiempo propio},\qquad
\Delta t=\gamma\Delta t_0.
$$

Despejes frecuentes:

$$
\Delta t_0=\frac{\Delta t}{\gamma},
\qquad
\gamma=\frac{\Delta t}{\Delta t_0},
\qquad
\frac{v}{c}=\sqrt{1-\frac{1}{\gamma^2}}.
$$

> [!note] Justificación física
> La relación sale de comparar la trayectoria vertical de un pulso de luz en el marco propio con su trayectoria diagonal en el marco donde el reloj se mueve. La derivación geométrica está en [[Teoría/02 - Conceptos de relatividad especial#Por qué aparece el factor de Lorentz]] y se visualiza en ![[imagenes/reloj-luz-dilatacion.svg]].

### Secuencia de decisión

1. ¿Cuáles son los dos eventos? Escríbelos.
2. ¿En qué marco suceden en el mismo lugar? Allí se mide $\Delta t_0$.
3. ¿Qué intervalo pide el problema: propio o medido desde el otro marco?
4. Calcula $\gamma$ y despeja antes de reemplazar datos.
5. Comprueba que $\Delta t\geq\Delta t_0$.

Si el enunciado dice que el tiempo exterior es 1 % mayor que el propio, tradúcelo como $\Delta t=1.01\Delta t_0$; entonces $\gamma=1.01$. Escribe esa interpretación antes de despejar $v/c$. Si “difiere 1 %” no aclara respecto de cuál valor, revisa la convención indicada en el enunciado o en clase.

## 3. Contracción de longitud

Para una longitud paralela al movimiento:

$$
L=\frac{L_0}{\gamma}.
$$

- $L_0$: longitud medida en el marco donde el objeto está en reposo.
- $L$: longitud medida en un marco donde el objeto se mueve.
- En cada marco, registra las posiciones de los extremos **simultáneamente en ese mismo marco**.
- La contracción solo afecta la dimensión paralela a la velocidad relativa.

Control: $L\leq L_0$. Si el problema da una dimensión transversal, no apliques esta ecuación a ella.

## 4. Suma relativista de velocidades colineales

Convención utilizada: el marco $S'$ se mueve a velocidad $+v$ respecto de $S$; $u'$ es la velocidad firmada del objeto en $S'$ y $u$ es su velocidad firmada en $S$.

$$
u=\frac{u'+v}{1+u'v/c^2}.
$$

Para invertir la relación:

$$
u'=\frac{u-v}{1-uv/c^2}.
$$

### Cómo asignar los signos

- Elige y dibuja el sentido $+x$.
- Una velocidad en $+x$ es positiva; una en $-x$, negativa.
- Dos objetos hacia el mismo sentido pueden tener signos positivos ambos.
- Si el proyectil se dispara hacia atrás desde una nave que se mueve en $+x$, entonces $u'<0$.
- El signo de $u$ informa el sentido final; su módulo debe ser menor que $c$.

### De dónde sale el denominador

Con la convención anterior, la transformación inversa de coordenadas es

$$
x=\gamma(x'+vt'),\qquad
t=\gamma\left(t'+\frac{vx'}{c^2}\right).
$$

Al derivar las coordenadas respecto del tiempo $t'$ medido en el marco móvil y dividir $dx/dt$, se obtiene

$$
u=\frac{dx}{dt}
=\frac{dx'/dt'+v}{1+(v/c^2)(dx'/dt')}
=\frac{u'+v}{1+u'v/c^2}.
$$

El término del denominador es la consecuencia de que también se transforma el tiempo; no es una corrección arbitraria. Para $v,u'\ll c$, el denominador tiende a 1 y se recupera aproximadamente la suma clásica.

## 5. Tiempo de llegada: no mezclar marcos

Después de hallar la velocidad del proyectil respecto de la Tierra, el tiempo terrestre de llegada se calcula con

$$
t=\frac{D}{u}.
$$

Esto solo es válido si $D$ y $u$ están medidos en el mismo marco. Convierte $D$ a metros y $u$ a m/s antes de calcular. Si el proyectil se mueve hacia la Tierra, usa su rapidez positiva en el eje dirigido hacia la Tierra.

## 6. Transformaciones de Lorentz y simultaneidad

Las relaciones de coordenadas que sustentan las transformaciones de velocidades son

$$
x'=\gamma(x-vt),\qquad
t'=\gamma\left(t-\frac{vx}{c^2}\right).
$$

Para dos eventos:

$$
\Delta t'=\gamma\left(\Delta t-\frac{v\,\Delta x}{c^2}\right).
$$

Si dos posiciones se registran al mismo tiempo en $S$ ($\Delta t=0$), en general $\Delta t'=-\gamma v\Delta x/c^2\neq0$: no son simultáneas en $S'$. Esta es la razón de fondo por la que cada marco debe hacer su propia medición simultánea de ambos extremos al medir una longitud. La explicación geométrica está en [[Teoría/02 - Conceptos de relatividad especial]] y en ![[imagenes/medicion-longitud-simultanea.svg]].

## 7. Errores que conviene prevenir

| Error | Cómo prevenirlo |
|---|---|
| Multiplicar por $\gamma$ un tiempo sin identificar los eventos | Marca el intervalo propio antes de calcular. |
| Llamar “propia” a la medición más larga por intuición | La propiedad depende del marco donde los eventos ocurren en el mismo lugar, no del valor dado. |
| Usar $L=L_0/\gamma$ sin revisar orientación | La regla debe medirse paralela al movimiento para que haya contracción. |
| Sumar velocidades clásicamente | Usa la transformación relativista y conserva signos. |
| Combinar distancia terrestre con velocidad medida desde la nave | Transforma primero la velocidad al marco terrestre. |
| Aceptar una rapidez mayor o igual que $c$ para el proyectil | Revisa signos, marcos y denominador. |

## Fuentes cotejadas

- [Capítulo de relatividad guardado en Zotero](zotero://select/library/items/YB8669CS): $\gamma$ y dilatación, PDF pp. 7–9; contracción, pp. 12–15; transformación de velocidades, pp. 17–19.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), p. 25: velocidades $0.400c$ y $0.700c$, y tiempo de alcance.
- [Resolución guardada del modelo 2024](zotero://select/library/items/UHEXA2AW): interpretación de la diferencia temporal del 1 %.

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

## 7. Extensión: energía relativista

> [!note] Prioridad
> El TP incluye energía relativista de electrones, pero ninguno de los modelos revisados la pregunta. Estúdiala después de tiempo propio, contracción y suma de velocidades.

La energía total de una partícula de masa $m$ que se mueve a rapidez $v$ es

$$
E=\gamma mc^2.
$$

En reposo, $\gamma=1$, así que su energía en reposo es $E_0=mc^2$. La energía cinética relativista es la diferencia:

$$
K=E-E_0=(\gamma-1)mc^2.
$$

Si la partícula parte del reposo y gana energía al cruzar una diferencia de potencial $\Delta V$, el trabajo del campo eléctrico es $K=|q|\,|\Delta V|$. Para un electrón, el valor numérico de la energía en eV coincide con la diferencia de potencial en voltios: por ejemplo, $20.0\,\mathrm{kV}$ le entrega $20.0\,\mathrm{keV}$.

Para hallar la rapidez a partir de la energía ganada:

$$
\gamma=1+\frac{K}{mc^2},\qquad
\frac{v}{c}=\sqrt{1-\frac{1}{\gamma^2}}.
$$

El paso $K=\frac12mv^2$ solo es una aproximación para $v\ll c$; no se usa para electrones acelerados a velocidades relativistas. Para el electrón, $m_ec^2\approx0.511\,\mathrm{MeV}$.

## 8. Errores que conviene prevenir

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
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), PDF pp. 22–24: energía en reposo, energía cinética relativista y rapidez de electrones acelerados.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), p. 25: velocidades $0.400c$ y $0.700c$, y tiempo de alcance.
- [Resolución guardada del modelo 2024](zotero://select/library/items/UHEXA2AW): interpretación de la diferencia temporal del 1 %.

## Autoevaluación de fórmulas

Antes de abrir cada explicación, escribe qué representa cada dato y en qué marco se mide.

**1. Un reloj viaja con una nave y mide el intervalo entre dos eventos que ocurren en el mismo lugar de la nave. ¿Qué relación usas para hallar el intervalo terrestre?**

> [!success]- Mostrar explicación
> El intervalo del reloj de la nave es propio: $\Delta t_0$. Primero calculas $\gamma=1/\sqrt{1-v^2/c^2}$ y luego usas $\Delta t=\gamma\Delta t_0$. El resultado terrestre debe ser igual o mayor que el propio. La elección se justifica por dónde ocurren los eventos, no por cuál valor es dado.

**2. Una nave mide 100 m en reposo y pasa paralela a su eje largo. ¿Qué longitud mide un observador que la ve moverse y qué sincronización requiere?**

> [!success]- Mostrar explicación
> Se usa $L=L_0/\gamma$. El observador registra las posiciones de ambos extremos al mismo tiempo en su propio marco; no puede tomar una lectura simultánea en el marco de la nave y reutilizarla. La contracción afecta solo la dirección paralela al movimiento.

**3. En $S'$, un proyectil viaja hacia $-x$ y el marco $S'$ se mueve hacia $+x$ respecto de $S$. ¿Cómo asignas los signos en $u=(u'+v)/(1+u'v/c^2)$?**

> [!success]- Mostrar explicación
> Escribes $u'<0$ porque el proyectil viaja hacia $-x$ en $S'$, y $v>0$ porque $S'$ se mueve hacia $+x$ respecto de $S$. Sustituyes esos signos en numerador y denominador; el signo de $u$ determina el sentido medido en $S$. El denominador aparece porque el tiempo también se transforma entre marcos, y el módulo de la velocidad resultante debe ser menor que $c$.

**4. ¿Puedes dividir una distancia medida desde la Tierra por una rapidez medida desde la nave para calcular el tiempo terrestre de llegada?**

> [!success]- Mostrar explicación
> No. La distancia y la rapidez deben corresponder al mismo marco para que $t=D/u$ describa el intervalo de ese observador. Primero transforma la velocidad al marco terrestre, convierte las unidades y entonces calcula el tiempo terrestre.

**5. Un electrón parte del reposo y gana energía cinética $K$ en una diferencia de potencial. ¿Cómo obtienes su rapidez sin usar $K=\frac12mv^2$?**

> [!success]- Mostrar explicación
> Primero usas $E_0=m_ec^2$ y $K=(\gamma-1)m_ec^2$, por lo que $\gamma=1+K/E_0$. Luego despejas $v/c=\sqrt{1-1/\gamma^2}$. La fórmula clásica de energía cinética no describe correctamente una partícula que se acerca a $c$.

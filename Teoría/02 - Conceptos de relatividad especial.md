---
tags: [fisica-aplicada, teoria, conceptos, relatividad]
---

# Conceptos — Relatividad especial

**Volver al módulo:** [[Teoría/02 - Relatividad especial]] · **Fórmulas y método:** [[Teoría/02 - Fórmulas aplicadas de relatividad especial]] · **Ejercicios:** [[Ejercicios/02 - Relatividad especial]]

## 1. Qué estudia la relatividad especial

La relatividad especial describe cómo se relacionan las mediciones de observadores que se mueven con velocidad constante entre sí. Cada observador usa un **marco de referencia**: un sistema de coordenadas y relojes sincronizados que permite asignar posición y tiempo a los acontecimientos.

Un **evento** es algo que sucede en un lugar y en un instante concretos: por ejemplo, encender un reflector o disparar un proyectil. Dos observadores pueden describir el mismo evento con coordenadas distintas. Para comparar sus mediciones hay que indicar siempre **qué marco** mide cada distancia, intervalo o velocidad.

El módulo se limita a marcos **inerciales** (sin aceleración) y a los tipos de problema del parcial. No incluye relatividad general ni efectos gravitatorios sobre el tiempo.

## 2. Los dos postulados y sus consecuencias

La teoría especial parte de dos postulados:

1. Las leyes de la física tienen la misma forma en todos los marcos inerciales.
2. La rapidez de la luz en el vacío es la misma para todos los observadores inerciales, sin depender del movimiento de la fuente.

En mecánica cotidiana se suman velocidades como si el tiempo fuera idéntico para todos. Esa regla no puede conservar simultáneamente los dos postulados cuando las velocidades se acercan a la de la luz. El espacio y el tiempo pasan a depender del marco; las fórmulas de este módulo expresan esa relación.

Usamos $c=3.00\times10^8\,\mathrm{m/s}$ como valor aproximado de la rapidez de la luz. Un objeto con masa no alcanza $c$.

## 3. El factor de Lorentz: cuánto importa el movimiento

Para una rapidez relativa $v$ entre marcos, definimos

$$
\gamma=\frac{1}{\sqrt{1-v^2/c^2}}.
$$

El cociente $v/c$ compara la rapidez con la de la luz. Por eso, al fijar una rapidez como fracción de $c$, el cálculo de $\gamma$ no requiere convertir primero a metros por segundo.

- Si $v=0$, entonces $\gamma=1$: las correcciones relativistas desaparecen.
- Si $v$ es mucho menor que $c$, $\gamma$ es muy cercano a 1 y las medidas casi coinciden con las clásicas.
- Cuando $v$ se aproxima a $c$, $\gamma$ crece mucho; los efectos de tiempo y longitud se vuelven apreciables.

$\gamma$ no es una corrección que se aplica a cualquier cantidad indistintamente. En estos ejercicios multiplica el tiempo propio y divide la longitud propia. Decidir **qué magnitud es propia** es el paso conceptual central.

## 4. Tiempo propio y dilatación temporal

El intervalo entre dos eventos depende del marco. El **tiempo propio**, $\Delta t_0$, es el intervalo medido en el marco donde ambos eventos ocurren en el mismo lugar. Un reloj que permanece junto a ese lugar puede registrar directamente los dos eventos.

Ejemplo: en la nave se enciende un reflector y, más tarde, se apaga. Si ambos eventos ocurren junto al mismo interruptor fijo en la nave, el reloj de la nave mide el tiempo propio. Desde la Tierra, la nave se desplaza; los dos eventos ocurren en posiciones terrestres distintas y se comparan usando relojes terrestres sincronizados.

La relación es

$$
\Delta t=\gamma\,\Delta t_0.
$$

### Por qué aparece el factor de Lorentz

Imagina un reloj que mide el tiempo contando el viaje de un pulso de luz entre una fuente y un espejo. En el marco donde el reloj está en reposo, la luz recorre una distancia $d$ en cada mitad del ciclo:

$$
\Delta t_0=\frac{2d}{c}.
$$

Desde otro marco, el reloj se desplaza horizontalmente durante el viaje. Para la mitad del recorrido, la luz sigue una diagonal: su componente vertical cubre $d$ y el aparato avanza $v\Delta t/2$. Como la luz conserva rapidez $c$, su trayecto mide $c\Delta t/2$. Aplicamos Pitágoras:

$$
\left(\frac{c\Delta t}{2}\right)^2
=d^2+\left(\frac{v\Delta t}{2}\right)^2.
$$

Sustituimos $d=c\Delta t_0/2$ y despejamos:

$$
c^2\Delta t^2=c^2\Delta t_0^2+v^2\Delta t^2,
\qquad
\Delta t=\frac{\Delta t_0}{\sqrt{1-v^2/c^2}}
=\gamma\Delta t_0.
$$

La trayectoria más larga requiere más tiempo porque ambos marcos miden la misma rapidez de la luz. El diagrama muestra un solo tramo; el recorrido de regreso tiene la misma geometría.

![[imagenes/reloj-luz-dilatacion.svg]]

El intervalo $\Delta t$ medido desde el marco donde el reloj se mueve es mayor que el tiempo propio. No es un retraso visual causado por el tiempo que tarda la luz en llegar al observador: las mediciones se corrigen para comparar cuándo ocurrieron los eventos, no cuándo se los ve.

**Cómo reconocerlo en un ejercicio:** escribe los dos eventos, por ejemplo “inicio” y “fin”; pregunta en qué marco suceden en el mismo lugar. El intervalo de ese marco es $\Delta t_0$. Después etiqueta como $\Delta t$ la medida del otro marco.

## 5. Longitud propia, medición simultánea y contracción

La **longitud propia**, $L_0$, es la longitud medida en el marco donde el objeto está en reposo. Para medir una longitud desde cualquier marco hay que registrar dónde están sus dos extremos **al mismo tiempo en ese marco**. En la Tierra, por ejemplo, se pueden usar dos reglas o relojes sincronizados situados junto a los extremos de la nave.

La simultaneidad no es absoluta: dos eventos simultáneos para la Tierra pueden no ser simultáneos para la nave. Por eso, al medir la nave en movimiento desde la Tierra, no se toma la separación entre dos sucesos escogidos simultáneamente en la nave; se registran las posiciones de ambos extremos en un mismo instante terrestre. La longitud paralela al movimiento resulta

$$
L=\frac{L_0}{\gamma}.
$$

La dimensión paralela al movimiento se contrae; las dimensiones perpendiculares no aparecen contraídas en este modelo. La diferencia no es una ilusión óptica. Las dos mediciones se hacen correctamente, pero utilizan distintos marcos y distintos pares de eventos simultáneos.

![[imagenes/medicion-longitud-simultanea.svg]]

## 6. Suma relativista de velocidades

La rapidez de un proyectil medida desde la nave no es, en general, la misma que mide la Tierra. La suma clásica podría predecir una rapidez superior a $c$, lo cual contradice el segundo postulado. Para movimiento en una sola recta se usa la transformación relativista, con signos:

$$
u=\frac{u'+v}{1+u'v/c^2}.
$$

Aquí $v$ es la velocidad de $S'$ respecto de $S$, $u'$ es la velocidad del objeto medida en $S'$, y $u$ es la velocidad medida en $S$. Se supone que $S'$ se desplaza en la dirección positiva respecto de $S$. Si el objeto se mueve en sentido contrario en $S'$, se escribe $u'<0$.

La ecuación cambia al invertir qué marco se considera móvil. Por eso conviene dibujar el eje y asignar signos **antes** de usarla. El resultado debe tener módulo menor que $c$.

## 7. Un límite útil: volver a la mecánica clásica

Cuando todas las velocidades son pequeñas comparadas con $c$, los términos $v^2/c^2$ y $u'v/c^2$ son pequeños. Entonces $\gamma\approx1$, los tiempos y longitudes casi coinciden, y la suma relativista se aproxima a $u\approx u'+v$.

Este límite permite entender por qué la mecánica clásica funciona tan bien en situaciones cotidianas y también sirve para detectar errores: si en un problema a $0.8c$ se obtiene exactamente la suma clásica, probablemente se aplicó el modelo equivocado.

## 8. Rutina conceptual antes de calcular

1. Dibuja los marcos y fija un eje positivo.
2. Nombra los eventos o los extremos que se miden.
3. Escribe debajo de cada dato quién lo mide.
4. Para tiempo: localiza el marco donde los dos eventos ocurren en el mismo punto.
5. Para longitud: identifica el marco de reposo y recuerda medir los extremos simultáneamente en el marco requerido.
6. Para velocidades: traduce las direcciones a signos algebraicos.
7. Recién entonces elige la fórmula de [[Teoría/02 - Fórmulas aplicadas de relatividad especial]].

## Fuentes de esta explicación

- [Capítulo de relatividad guardado en Zotero](zotero://select/library/items/YB8669CS): postulados y simultaneidad, PDF pp. 1–6; tiempo propio y dilatación, pp. 7–9; longitud, pp. 12–15; transformaciones de Lorentz y velocidad, pp. 17–19.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK): identificación del tiempo propio en el ejemplo inicial, p. 8; transformación de velocidades y alcance, p. 25.
- El detalle de páginas y su relación con los modelos está en [[Fuentes Zotero y probabilidad#Relatividad especial: fuentes consultadas para el módulo]].

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

### Por qué no basta con la transformación clásica

Supongamos que el marco $S'$ se mueve en la dirección $+x$ con rapidez $v$ respecto de $S$. La transformación clásica supone que ambos marcos comparten el mismo tiempo: $t'=t$, y relaciona las posiciones mediante $x'=x-vt$. Al derivar se obtiene la suma clásica de velocidades. Para un rayo que avanza en $+x$, esa regla predeciría $c'=c-v$ (o $c+v$, según cuál marco se despeje), aunque el segundo postulado exige que ambos observadores midan $c$. La contradicción muestra que no se puede conservar el supuesto de un tiempo universal.

La transformación de Lorentz ajusta conjuntamente posición y tiempo:

$$
x'=\gamma(x-vt),\qquad t'=\gamma\left(t-\frac{vx}{c^2}\right).
$$

El término con $x$ en la ecuación del tiempo hace que dos sucesos separados puedan dejar de ser simultáneos al cambiar de marco. Como comprobación, si la luz sigue $x=ct$, entonces $x'/t'=c$ también: la transformación conserva la rapidez de la luz.

![[imagenes/suma-galileana-y-luz-libro.png|900]]

> [!info] Figura 37.2 del libro, PDF p. 3 (p. 1270 del libro)
> La suma clásica funciona como aproximación para el misil lento, pero predice una rapidez mayor que $c$ para la luz. La figura muestra por qué se necesitan relaciones relativistas entre las coordenadas.

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

## 5. Simultaneidad, longitud propia y contracción

### Qué significa que dos sucesos sean simultáneos

Un suceso queda identificado por un lugar y un instante. Para decidir si dos sucesos separados ocurrieron al mismo tiempo, un observador necesita relojes sincronizados ubicados en esos lugares; comparar cuándo le llega la luz al ojo no basta, porque los tiempos de viaje pueden diferir.

El experimento del tren ayuda a ver por qué la respuesta depende del marco. Sergio está quieto en el suelo, a igual distancia de los dos puntos donde caen los rayos. Si las señales llegan juntas a Sergio y él corrige el tiempo de propagación con su red de relojes sincronizados, concluye que los impactos fueron simultáneos en el marco terrestre. Magda viaja en el tren hacia uno de los frentes luminosos y se aleja del otro. Como ambos frentes viajan a rapidez $c$, ella recibe primero el que viene de adelante; usando sus propios relojes sincronizados, concluye que ese impacto ocurrió antes. Ninguno está usando un reloj defectuoso: los observadores asignan tiempos distintos a los mismos sucesos porque se mueven uno respecto del otro.

![[imagenes/experimento-tren-simultaneidad-libro.png|720]]

> [!info] Figura 37.5 del libro, PDF p. 6 (p. 1273 del libro)
> Los dibujos distinguen los impactos de los momentos en que cada observador recibe la luz. La conclusión sobre simultaneidad requiere corregir el tiempo de viaje y usar relojes sincronizados en cada marco.

La transformación de Lorentz expresa esta diferencia para dos sucesos:

$$
\Delta t'=\gamma\left(\Delta t-\frac{v\,\Delta x}{c^2}\right).
$$

Si Sergio mide los impactos simultáneamente, $\Delta t=0$. Para impactos separados en la dirección del movimiento, $\Delta x\ne0$, resulta $\Delta t'=-\gamma v\Delta x/c^2\ne0$. Por tanto, la simultaneidad no es absoluta: depende del marco que asigna los tiempos.

### De la simultaneidad a la contracción de longitud

La **longitud propia**, $L_0$, es la longitud medida en el marco donde el objeto está en reposo. Para medir una longitud desde cualquier marco hay que registrar dónde están sus dos extremos **al mismo tiempo en ese marco**. En la Tierra, por ejemplo, se pueden usar dos reglas o relojes sincronizados situados junto a los extremos de la nave.

La contracción se obtiene de la transformación de Lorentz, no de una regla independiente. Llamemos $S'$ al marco donde la nave está quieta y $S$ al marco terrestre, desde el que la nave se mueve en $+x$ con rapidez $v$. Para los dos eventos que registran los extremos, la Tierra exige simultaneidad: $\Delta t=0$. Entonces,

$$
\Delta x'=\gamma(\Delta x-v\Delta t)=\gamma\Delta x.
$$

En el marco $S'$, los extremos están fijos; por eso su separación coordenada es la longitud propia $L_0=\Delta x'$. En el marco terrestre, la separación medida es $L=\Delta x$. De $L_0=\gamma L$ se obtiene

$$
L=\frac{L_0}{\gamma}=L_0\sqrt{1-\frac{v^2}{c^2}}.
$$

Los eventos usados por la Tierra suelen no ser simultáneos en $S'$, pero eso no cambia la separación entre los extremos porque la nave permanece en reposo allí. En cambio, cada marco debe usar su propia pareja de eventos simultáneos para medir longitud. La contracción afecta la dimensión paralela al movimiento; las dimensiones perpendiculares no aparecen contraídas en este modelo. No es una ilusión óptica: es una diferencia entre mediciones espaciales bien definidas en marcos distintos.

![[imagenes/medicion-longitud-simultanea.svg]]

## 6. Suma relativista de velocidades

La rapidez de un proyectil medida desde la nave no es, en general, la misma que mide la Tierra. La suma clásica podría predecir una rapidez superior a $c$, lo cual contradice el segundo postulado. Para movimiento en una sola recta se usa la transformación relativista, con signos:

$$
u=\frac{u'+v}{1+u'v/c^2}.
$$

Aquí $v$ es la velocidad de $S'$ respecto de $S$, $u'$ es la velocidad del objeto medida en $S'$, y $u$ es la velocidad medida en $S$. Se supone que $S'$ se desplaza en la dirección positiva respecto de $S$. Si el objeto se mueve en sentido contrario en $S'$, se escribe $u'<0$.

La ecuación cambia al invertir qué marco se considera móvil. Por eso conviene dibujar el eje y asignar signos **antes** de usarla. El resultado debe tener módulo menor que $c$.

### De dónde sale la suma relativista

Las coordenadas no se transforman por separado: también cambia el intervalo de tiempo. Con la convención de arriba, la transformación inversa es

$$
\Delta x=\gamma(\Delta x'+v\Delta t'),\qquad
\Delta t=\gamma\left(\Delta t'+\frac{v\Delta x'}{c^2}\right).
$$

Al dividir desplazamiento por tiempo y escribir $u'=\Delta x'/\Delta t'$, se obtiene $u=(u'+v)/(1+u'v/c^2)$. El denominador aparece porque $\Delta t$ también depende del desplazamiento $\Delta x'$; no es una corrección añadida a mano. Si $u'=c$, la expresión devuelve $u=c$, como requieren los postulados. El despeje algebraico paso a paso está en [[Teoría/02 - Fórmulas aplicadas de relatividad especial#4. Suma relativista de velocidades colineales]].

## 7. Un límite útil: volver a la mecánica clásica

Cuando todas las velocidades son pequeñas comparadas con $c$, los términos $v^2/c^2$ y $u'v/c^2$ son pequeños. Entonces $\gamma\approx1$, los tiempos y longitudes casi coinciden, y la suma relativista se aproxima a $u\approx u'+v$.

La primera diferencia respecto del resultado clásico aparece en el orden $\beta^2$, donde $\beta=v/c$. Con la aproximación binomial $(1-x)^{-1/2}\approx1+x/2$ para $x\ll1$,

$$
\gamma\approx1+\frac{\beta^2}{2},\qquad
\Delta t_0=\frac{\Delta t}{\gamma}\approx\Delta t\left(1-\frac{\beta^2}{2}\right).
$$

Por eso, a velocidades cotidianas el efecto puede ser real pero demasiado pequeño para aparecer en un resultado redondeado; el vuelo del ejercicio C7 practica cómo estimar esa corrección.

Este límite permite entender por qué la mecánica clásica funciona tan bien en situaciones cotidianas y también sirve para detectar errores: si en un problema a $0.8c$ se obtiene exactamente la suma clásica, probablemente se aplicó el modelo equivocado.

## 8. Extensión: energía relativista

Los ejercicios principales del parcial revisado se resuelven con intervalos, longitudes y velocidades. El TP agrega un caso de electrones acelerados que requiere energía relativista, pero este tipo no aparece en los modelos analizados.

La energía en reposo de una partícula es $E_0=mc^2$. Cuando se mueve, su energía total es $E=\gamma mc^2$; la diferencia $K=E-E_0=(\gamma-1)mc^2$ es la energía cinética. Si un electrón parte del reposo y atraviesa una diferencia de potencial, el campo eléctrico le entrega una energía $K=e|\Delta V|$. Se despeja $\gamma=1+K/(m_ec^2)$ y luego $v/c=\sqrt{1-1/\gamma^2}$.

Esta relación explica por qué la rapidez de un electrón crece cada vez menos al aumentar mucho la energía: $v$ se acerca a $c$ sin alcanzarla. Para un electrón, $m_ec^2\approx0.511\,\mathrm{MeV}$. La derivación operativa y el ejemplo están en [[Teoría/02 - Fórmulas aplicadas de relatividad especial#7. Extensión: energía relativista]] y [[Resoluciones/02 - Relatividad especial#C5. Energía y rapidez de electrones]].

## 9. Rutina conceptual antes de calcular

1. Dibuja los marcos y fija un eje positivo.
2. Nombra los eventos o los extremos que se miden.
3. Escribe debajo de cada dato quién lo mide.
4. Para tiempo: localiza el marco donde los dos eventos ocurren en el mismo punto.
5. Para longitud: identifica el marco de reposo y recuerda medir los extremos simultáneamente en el marco requerido.
6. Para velocidades: traduce las direcciones a signos algebraicos.
7. Recién entonces elige la fórmula de [[Teoría/02 - Fórmulas aplicadas de relatividad especial]].

## Fuentes de esta explicación

- [Capítulo de relatividad guardado en Zotero](zotero://select/library/items/YB8669CS): postulados y límite de la transformación galileana, PDF pp. 1–4 (Fig. 37.2, p. 3); simultaneidad (Fig. 37.5), p. 6; tiempo propio y dilatación, pp. 7–9; longitud, pp. 12–15; transformación de Lorentz y velocidades, pp. 16–19.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK), PDF pp. 22–24: energía relativista de electrones como extensión del TP.
- [Problemas de relatividad aplicada](zotero://select/library/items/N655C6SK): identificación del tiempo propio en el ejemplo inicial, p. 8; transformación de velocidades y alcance, p. 25.
- El detalle de páginas y su relación con los modelos está en [[Fuentes Zotero y probabilidad#Relatividad especial: fuentes consultadas para el módulo]].

## Autoevaluación de conceptos

Responde cada pregunta por tu cuenta y despliega después su explicación razonada.

**1. ¿Qué afirma el segundo postulado de la relatividad especial y qué límite impone a la suma de velocidades?**

> [!success]- Mostrar explicación
> La rapidez de la luz en el vacío es la misma para todo observador inercial, independientemente del movimiento de la fuente. Si se conservara el tiempo universal de la transformación clásica, la suma de velocidades daría $c+v$ o $c-v$ para un rayo, en contradicción con ese postulado. La transformación de Lorentz cambia cómo se relacionan espacio y tiempo entre marcos y mantiene $c$ invariante. Para velocidades mucho menores que $c$, se recupera aproximadamente la mecánica clásica.

**2. ¿Qué hace que un intervalo sea tiempo propio y por qué otro marco mide un intervalo mayor?**

> [!success]- Mostrar explicación
> Los dos eventos deben ocurrir en el mismo lugar del marco que mide $\Delta t_0$. En otro marco el reloj se mueve y los eventos ocurren en posiciones distintas. Al comparar las mediciones, $\Delta t=\gamma\Delta t_0$ con $\gamma>1$ si hay movimiento relativo; la diferencia surge de la geometría espacio-temporal, no de un defecto del reloj.

**3. ¿Por qué una medición de longitud requiere que los extremos se registren simultáneamente en el marco que mide?**

> [!success]- Mostrar explicación
> La longitud es la separación entre los extremos en un mismo instante del marco que mide. La relación $\Delta t'=\gamma(\Delta t-v\Delta x/c^2)$ muestra que dos registros simultáneos en la Tierra ($\Delta t=0$) no suelen ser simultáneos en la nave ($\Delta t'\ne0$). La longitud propia se mide en el marco de reposo del objeto; al medir simultáneamente los extremos desde un marco donde se mueve, se obtiene $L=L_0/\gamma$ en la dirección del movimiento.

**4. Una nave avanza hacia $+x$ y lanza un proyectil hacia atrás. ¿Qué signo tiene la velocidad del proyectil en el marco de la nave y para qué sirve ese signo?**

> [!success]- Mostrar explicación
> Si se define $+x$ como la dirección de avance de la nave, el proyectil tiene $u'<0$ en el marco de ella. El signo permite aplicar la suma relativista con la orientación correcta y decidir si, desde la Tierra, el proyectil todavía avanza hacia $+x$ o termina moviéndose hacia $-x$.

**5. ¿Qué energía gana un electrón que parte del reposo al atravesar una diferencia de potencial, y cómo se convierte esa energía en rapidez?**

> [!success]- Mostrar explicación
> El trabajo eléctrico aporta $K=e|\Delta V|$. Se relaciona con la energía relativista mediante $K=(\gamma-1)m_ec^2$; se despeja $\gamma$ y luego $v/c=\sqrt{1-1/\gamma^2}$. Este contenido es una ampliación del TP, posterior a los tipos que aparecen en los modelos.

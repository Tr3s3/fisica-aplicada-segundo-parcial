---
tags: [fisica-aplicada, teoria, gravitacion, conceptos]
---

# Conceptos — Gravitación y órbitas

**Recorrido:** [[Teoría/01 - Gravitación y órbitas|Índice]] · [[Teoría/01 - Fórmulas aplicadas de gravitación y órbitas|Fórmulas]] · [[Ejercicios/01 - Gravitación y órbitas|Práctica]] · [[Resoluciones/01 - Gravitación y órbitas|Resoluciones]]

Esta nota desarrolla el hilo físico que conecta los conceptos con las ecuaciones. Para cada relación, busca responder tres preguntas: **qué describe**, **de qué idea sale** y **qué supuesto permite usarla**. Después de comprender ese hilo, usa la nota de [[Teoría/01 - Fórmulas aplicadas de gravitación y órbitas]] como formulario de cálculo.

## Qué debes poder explicar

- Qué expresa la ley universal de gravitación y por qué la distancia se mide entre centros.
- Cómo se pasa de fuerza gravitatoria a campo y luego a peso.
- Por qué la contribución de varias masas se suma como vector.
- Qué cambia al subir sobre un planeta o al medir el peso en un planeta que rota.
- Cómo la gravedad puede mantener un satélite en caída libre alrededor del planeta.
- De dónde salen la energía potencial gravitatoria, la energía de una órbita y la rapidez de escape.
- Qué relación descubrió Kepler y bajo qué condición se puede comparar una órbita con otra.

## 0. El modelo que vamos a usar

La gravitación newtoniana es un modelo para describir la atracción entre masas. En estos ejercicios se supone que las velocidades son mucho menores que la rapidez de la luz y que los campos gravitatorios no son tan intensos como para requerir relatividad.

### De la observación a la ley de Newton

Newton reunió en una sola ley fenómenos que antes parecían distintos: la caída de los objetos cerca de la Tierra y el movimiento de la Luna y los planetas. La ley establece dos dependencias:

1. Si aumenta cualquiera de las masas, aumenta la fuerza; la fuerza es proporcional al producto de las masas.
2. Si aumenta la distancia entre los centros, la fuerza disminuye como el cuadrado de esa distancia.

Al reunirlas, para dos masas puntuales se obtiene la magnitud

$$
F_g=G\frac{Mm}{r^2}.
$$

![[imagenes/ley-gravitacion-dos-masas-libro.png|500]]

*Figura 12.1, recortada del capítulo 12, p. 384 (PDF, p. 2). Cada masa atrae a la otra a lo largo de la línea que las une; las dos fuerzas tienen igual módulo y sentidos opuestos.*

Esta relación es la **ley universal de gravitación**. En este nivel no se deduce de la fórmula de la órbita circular: es la ley de interacción que se combina con las leyes de Newton para explicar caídas y órbitas. La constante $G$ fija la intensidad de la interacción y se determina experimentalmente. Se llama universal porque su valor no depende del lugar: es el mismo en la Tierra, Marte o el espacio. Cavendish la midió con una balanza de torsión, observando la atracción diminuta entre esferas de masas y separación conocidas.

![[imagenes/balanza-cavendish-libro.png|800]]

*Figura 12.4, recortada del capítulo 12, p. 385 (PDF, p. 3). La atracción entre masas desplaza una varilla suspendida; la desviación amplificada por el láser permite medir la fuerza y determinar $G$.*

- $M$ y $m$: masas que se atraen, en kilogramos.
- $r$: distancia entre sus centros, en metros.
- $G\approx6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.
- $F_g$: módulo de la fuerza, en newtons.

La dependencia $1/r^2$ permite anticipar cómo cambia la fuerza sin recalcular todo: al duplicar $r$, la fuerza queda en $1/4$; al triplicar $r$, queda en $1/9$. La fuerza siempre apunta a lo largo de la línea que une los centros y es atractiva.

> [!important] Magnitud y dirección son dos partes del modelo
> La fórmula anterior calcula el **módulo**. Para saber hacia dónde apunta, dibuja la línea entre las masas: cada cuerpo es atraído hacia el otro. Las dos fuerzas de interacción tienen igual módulo y sentidos opuestos, aunque las aceleraciones que producen pueden ser distintas porque $a=F/m$ y las masas pueden diferir.

### Cuándo puede tratarse un cuerpo como una masa puntual

La ley se formula primero para masas puntuales. El teorema de las capas esféricas permite extenderla a una esfera con distribución de masa esféricamente simétrica: aunque la esfera esté hecha de muchas partes, sus atracciones se combinan de modo que, **en un punto exterior**, el resultado es igual al de toda la masa concentrada en el centro. Por eso, para un objeto sobre la superficie o a cierta altura, usamos la distancia del objeto al centro del planeta.

![[imagenes/simetria-esferica-masa-puntual-libro.png|500]]

*Figura 12.2, recortada del capítulo 12, p. 384 (PDF, p. 2). Para puntos exteriores, la fuerza entre dos cuerpos esféricamente simétricos se calcula como si sus masas estuvieran concentradas en sus centros.*

Este reemplazo no se aplica automáticamente a puntos dentro del planeta. Tampoco se debe medir $r$ desde la superficie si el enunciado entrega una altura.

> [!abstract] Supuestos frecuentes en estos ejercicios
> - Se modelan los planetas y estrellas como esferas simétricas vistas desde fuera.
> - Si se estudia un planeta aislado, se ignora la atracción de otros cuerpos.
> - Para una órbita circular ideal, solo actúa la gravedad; se desprecian el aire y los empujes.
> - Para comparar órbitas planetarias, la masa del planeta que orbita es pequeña frente a la masa central.
> - La rapidez de escape es el umbral para llegar muy lejos con rapidez final tendiendo a cero, sin resistencia del aire ni aporte posterior de energía.

## 1. De fuerza gravitatoria a campo y peso

### Fuerza: interacción entre dos masas

En la ley de gravitación, $M$ puede ser el planeta y $m$ un objeto cercano. El módulo es

$$
F_g=G\frac{Mm}{r^2}.
$$

La fuerza sobre el objeto $m$ apunta hacia el centro de $M$. Si definimos $\hat{\mathbf r}$ como una flecha unitaria que apunta desde el centro de la fuente hacia afuera, la forma vectorial es

$$
\vec F_g=-G\frac{Mm}{r^2}\hat{\mathbf r}.
$$

El signo menos indica que la fuerza apunta en sentido contrario a $\hat{\mathbf r}$, es decir, hacia la fuente.

### Campo: describir lo que la fuente produce en cada punto

A veces interesa conocer primero el efecto del planeta en un punto, sin elegir todavía qué objeto colocaremos allí. Para eso definimos el **campo gravitatorio** como la fuerza por unidad de masa de prueba:

$$
\vec g=\frac{\vec F_g}{m}.
$$

Al sustituir la ley de gravitación, la masa de prueba se cancela:

$$
\vec g
=\frac{-GMm\,\hat{\mathbf r}/r^2}{m}
=-G\frac{M}{r^2}\hat{\mathbf r}.
$$

Por lo tanto, el módulo del campo de una fuente es

$$
g=G\frac{M}{r^2}.
$$

La cancelación explica dos hechos:

- El campo en un punto depende de la masa que lo produce y de la distancia a ella, no del objeto de prueba.
- Si solo actúa la gravedad, la aceleración del objeto es $\vec a=\vec F_g/m=\vec g$. Dos objetos de masas distintas reciben la misma aceleración gravitatoria en el mismo punto, aunque las fuerzas sobre ellos tengan distinto módulo.

La unidad del campo puede escribirse $\mathrm{N/kg}$ o $\mathrm{m/s^2}$: son equivalentes porque $1\,\mathrm{N}=1\,\mathrm{kg\,m/s^2}$. No confundas $G$, que es una constante universal, con $g$, que es el campo local y cambia de un lugar a otro.

![[imagenes/campo-gravitatorio.svg]]

### Peso: la fuerza gravitatoria sobre un objeto

La fuerza gravitatoria sobre una masa cercana a un planeta se llama su **peso gravitatorio**:

$$
\vec W=\vec F_g=m\vec g,
\qquad
W=mg \quad\text{para los módulos}.
$$

La masa mide la inercia y se conserva al trasladar el objeto. El peso es una fuerza, así que cambia si cambia el campo. Por ejemplo, el mismo objeto tiene pesos distintos en la superficie de la Tierra y de Marte.

Cerca de la superficie terrestre solemos usar $g\approx9.8\,\mathrm{m/s^2}$, pero ese valor es una aproximación local. Para calcularlo desde la masa y el radio del planeta se combina la ley de Newton con la definición de campo:

$$
g_{\text{superficie}}
=\frac{F_g}{m}
=\frac{GMm/R^2}{m}
=\frac{GM}{R^2}.
$$

Aquí $R$ es el radio del planeta y $M$ su masa. La última expresión muestra cómo la gravedad superficial depende de la masa y del tamaño del planeta.

## 2. Varias masas: los campos se suman como flechas

Si varias masas atraen al mismo objeto, cada una produce su campo. En el modelo newtoniano, las contribuciones de las fuentes se calculan por separado y la fuerza neta es su resultante. El principio de superposición dice que el campo total es la suma vectorial:

$$
\vec g_{\text{total}}=\sum_i\vec g_i.
$$

La fuerza total sobre una masa de prueba $m$ es entonces

$$
\vec F_{\text{total}}=m\vec g_{\text{total}}.
$$

Esto convierte un problema de muchas fuerzas en una suma ordenada:

1. Marca el punto donde se busca el campo y dibuja una flecha desde ese punto hacia cada masa fuente.
2. Calcula cada módulo con $g_i=GM_i/r_i^2$.
3. Asigna ejes y descompón las flechas en componentes con signo.
4. Suma primero las componentes; recién al final calcula el módulo y la dirección del resultado.

En dos dimensiones,

$$
g_x=\sum_i g_{ix},
\qquad
g_y=\sum_i g_{iy},
\qquad
|\vec g|=\sqrt{g_x^2+g_y^2}.
$$

Si dos componentes horizontales son iguales y opuestas, se cancelan. Si apuntan en el mismo sentido, se suman. La simetría puede simplificar el cálculo, pero hay que justificarla mirando la geometría.

El ejemplo del libro muestra la suma de dos fuerzas sobre una estrella pequeña. La resultante se obtiene sumando las componentes de cada vector, no agregando directamente sus módulos.

![[imagenes/superposicion-fuerzas-gravitatorias-libro.png|750]]

*Figura 12.5, recortada del capítulo 12, p. 386 (PDF, p. 4). Las fuerzas $\vec F_1$ y $\vec F_2$ se combinan para producir la fuerza total $\vec F$.*

![[imagenes/campo-no-simetrico.svg]]

> [!example] Qué significa que el campo total sea cero
> En un punto donde dos campos se cancelan, la fuerza gravitatoria neta sobre una masa de prueba también es cero en ese instante. Cada fuente sigue atrayéndola; el resultado cero aparece por la suma de fuerzas opuestas, no porque haya desaparecido la gravedad.

## 3. Altura: por qué usamos $R+h$

La ley de gravitación necesita la distancia entre centros. Para un objeto a altura $h$ sobre un planeta de radio $R$, el radio de la trayectoria desde el centro es

$$
r=R+h.
$$

![[imagenes/orbita-satelite.svg|700]]

*Esquema del vault: la distancia orbital $r$ parte del centro y se compone del radio del planeta $R$ más la altura $h$.*

Al sustituirlo en la expresión del campo,

$$
g(h)=\frac{GM}{(R+h)^2}.
$$

En la superficie, $g_0=GM/R^2$. Dividir ambas expresiones permite comparar el campo a la altura $h$ con el de la superficie sin conocer $G$ ni $M$:

$$
\frac{g(h)}{g_0}
=\frac{GM/(R+h)^2}{GM/R^2}
=\left(\frac{R}{R+h}\right)^2.
$$

Para el mismo objeto, $W=mg$, de modo que el cociente de pesos es igual al cociente de campos:

$$
\frac{W(h)}{W_0}=\frac{g(h)}{g_0}.
$$

**Ejemplo de interpretación.** Si $h=R$, el objeto está a $2R$ del centro. Entonces $g(h)/g_0=(R/2R)^2=1/4$. La altura no es el radio que se introduce directamente en la ley: primero se suma al radio del planeta.

### Por qué cerca del suelo se suele usar $W=mg$ con $g$ constante

Cuando la altura es pequeña comparada con $R$, la distancia al centro cambia muy poco durante el movimiento. El campo también cambia muy poco, y podemos aproximarlo por su valor superficial constante. Esta aproximación sirve para movimientos cotidianos cerca del suelo; para satélites o grandes alturas conviene conservar la dependencia con $r$.

La aproximación local $mgh$ para la energía potencial se obtiene con más detalle en la sección 7.

## 4. Peso aparente en el ecuador de un planeta que rota

Una balanza no mide directamente la atracción gravitatoria; mide la fuerza normal $N$ que ejerce sobre la persona. En el ecuador de un planeta que rota, una persona fija respecto del suelo describe una circunferencia y necesita una aceleración centrípeta dirigida hacia el centro.

Tomamos hacia el centro como sentido positivo. Actúan dos fuerzas radiales sobre la persona: la gravedad $mg$ hacia adentro y la normal $N$ de la balanza hacia afuera. La segunda ley de Newton da

$$
mg-N=ma_c.
$$

Al dividir por la masa de la persona,

$$
g_{\text{aparente}}
=\frac{N}{m}
=g-a_c
=\frac{GM}{R^2}-\frac{v^2}{R}.
$$

Si el planeta tarda un tiempo $T$ en completar una rotación, su rapidez angular es $\omega=2\pi/T$ y la aceleración centrípeta en el ecuador también puede escribirse $a_c=\omega^2R=4\pi^2R/T^2$. Así se ve de dónde sale la corrección por rotación: la gravedad no desaparece; una parte de la fuerza neta requerida la proporciona la propia aceleración del movimiento circular.

![[imagenes/gravedad-rotacion-jupiter.svg]]

El resultado es una lectura de balanza menor que el peso gravitatorio $mg$. Esta fórmula corresponde al ecuador y a un modelo esférico; en latitudes distintas la geometría del movimiento es diferente. El ejercicio de Júpiter del TP usa precisamente esta corrección.

## 5. Órbita circular: caída libre alrededor del planeta

### De un proyectil a un satélite

Imagina lanzar un proyectil horizontalmente desde una montaña muy alta. La gravedad curva su camino hacia la Tierra. Si se lanza con más rapidez, avanza más antes de tocar el suelo. A gran altura la superficie terrestre también se curva; si el proyectil avanza lo suficiente mientras cae, la superficie puede curvarse alejándose a la misma tasa. Entonces el proyectil sigue cayendo alrededor de la Tierra y queda en órbita.

![[imagenes/trayectorias-orbitales-libro.png|750]]

*Figura 12.14, recortada del capítulo 12, p. 393 (PDF, p. 11). Las trayectorias muestran cómo cambia el resultado al aumentar la rapidez de lanzamiento; el dibujo supone que no hay resistencia del aire.*

La imagen ayuda a entender que una órbita es una forma de caída libre: la gravedad sigue desviando el movimiento hacia la Tierra, pero la velocidad tangencial evita que el satélite llegue al suelo. En la órbita circular ideal, la distancia al centro se mantiene constante.

### Velocidad tangencial: de arco a rapidez

La **velocidad instantánea** indica hacia dónde se mueve el objeto en ese instante. Durante un intervalo finito, el objeto avanza una cuerda entre dos puntos de la órbita; al hacer ese intervalo cada vez más corto, la cuerda se aproxima a la tangente. Por eso la velocidad instantánea es tangente a la circunferencia y perpendicular al radio.

La distancia recorrida sobre el borde es un arco. Si el ángulo $\theta$ está medido en radianes, la definición del radián da $s=r\theta$. Entonces la rapidez tangencial, que es cuánto arco recorre por unidad de tiempo, se obtiene así:

$$
v_t=\frac{ds}{dt}
=r\left|\frac{d\theta}{dt}\right|
=r\omega.
$$

Aquí $\omega=|d\theta/dt|$ es la rapidez angular, medida en radianes por segundo. Esta relación vale en cada instante para un movimiento circular de radio fijo. Si el movimiento es uniforme y una vuelta tarda un período $T$, el objeto recorre una circunferencia completa $2\pi r$ en ese tiempo:

$$
\omega=\frac{2\pi}{T},
\qquad
v_t=\frac{2\pi r}{T}.
$$

Si la rapidez cambia durante la vuelta, $2\pi r/T$ da la rapidez tangencial media; la relación instantánea sigue siendo $v_t=r\omega$. En la órbita circular, $v_t$ es la rapidez orbital. La velocidad es tangente, mientras que el radio apunta desde el centro hasta el satélite.

### Aceleración centrípeta: del cambio de velocidad al radio

La **velocidad** es un vector, así que puede cambiar aunque su módulo permanezca constante. En el movimiento circular uniforme, dos velocidades en instantes cercanos tienen igual módulo $v_t$, pero direcciones distintas. El radio también gira un ángulo pequeño $\Delta\theta$ entre esos instantes; las tangentes giran el mismo ángulo.

Al dibujar las dos velocidades con un origen común, la diferencia $\Delta\vec v=\vec v_B-\vec v_A$ es el tercer lado de un triángulo. Su módulo es la cuerda de un círculo de radio $v_t$:

$$
|\Delta\vec v|
=2v_t\sin\left(\frac{\Delta\theta}{2}\right)
\approx v_t\Delta\theta
\quad\text{si }\Delta\theta\text{ es pequeño}.
$$

El símbolo $\lim_{\Delta t\to0}$ indica que hacemos el intervalo cada vez más corto para obtener la aceleración instantánea. En ese límite, el arco recorrido cumple $\Delta s\approx r\Delta\theta$ y $\Delta s/\Delta t$ se aproxima a la rapidez $v_t=v$. Por eso:

![[imagenes/velocidad-tangencial-cambio-velocidad.svg|900]]

*Esquema propio. A la izquierda se ve que la velocidad sigue la tangente; a la derecha, el cambio entre dos vectores velocidad de igual módulo apunta aproximadamente hacia el centro.*

$$
a_c
=\lim_{\Delta t\to0}\frac{|\Delta\vec v|}{\Delta t}
=\lim_{\Delta t\to0}\frac{v_t\Delta\theta}{\Delta t}
=\frac{v_t}{r}\lim_{\Delta t\to0}\frac{\Delta s}{\Delta t}
=\frac{v_t^2}{r}.
$$

La diferencia $\Delta\vec v$ apunta hacia el centro cuando el intervalo se hace muy pequeño; por eso también lo hace esta componente de la aceleración. Se llama **aceleración centrípeta**: “centrípeta” significa dirigida hacia el centro. La fórmula $a_c=v_t^2/r$ da la componente radial de la aceleración en una trayectoria circular. Si la rapidez también cambia, aparece además una componente tangencial $a_t=dv_t/dt$; en el movimiento circular uniforme, $a_c$ es toda la aceleración.

### De la aceleración a la fuerza centrípeta

La segunda ley de Newton relaciona la aceleración con la **fuerza neta** que la produce: $\sum\vec F=m\vec a$. Para conservar una trayectoria circular, la componente radial neta debe apuntar hacia el centro y tener módulo

$$
F_c=ma_c=m\frac{v_t^2}{r}.
$$

La expresión **fuerza centrípeta** nombra el papel de esa fuerza neta hacia adentro; no describe una interacción adicional. En el modelo de una órbita circular aislada, la única fuerza radial es la atracción gravitatoria, así que la gravedad hace ese papel.

![[imagenes/orbita-circular-fuerza-centripeta-libro.png|500]]

*Figura 12.15, recortada del capítulo 12, p. 394 (PDF, p. 12). En cada posición, la velocidad $\vec v$ es tangente a la órbita; la fuerza gravitatoria $\vec F_g$ y la aceleración $\vec a$ apuntan hacia el centro.*

Al mirar los vectores de la figura:

1. $\vec v$ apunta a lo largo de la tangente, así que es perpendicular al radio.
2. $\vec F_g$ apunta al centro porque la gravedad es atractiva.
3. $\vec a$ apunta en la misma dirección que la fuerza neta, según la segunda ley de Newton.
4. Como $\vec a$ es perpendicular a $\vec v$, cambia la dirección de la velocidad, no su módulo; por eso el movimiento circular puede tener rapidez constante.

Igualamos ahora la gravedad con la fuerza radial neta requerida para la órbita:

$$
\sum F_r=ma_c,
\qquad
G\frac{Mm}{r^2}=m\frac{v^2}{r}.
$$

Se cancela la masa del satélite $m$, porque aparece en ambos lados. Al despejar $v$:

$$
v_{\text{orb}}^2=\frac{GM}{r},
\qquad
v_{\text{orb}}=\sqrt{\frac{GM}{r}}.
$$

La rapidez orbital depende de la masa central $M$ y del radio orbital $r$, pero no de la masa del satélite. Esto ocurre porque una masa mayor siente una fuerza gravitatoria proporcionalmente mayor, pero también necesita proporcionalmente más fuerza para producir la misma aceleración.

Para hallar el período, usamos que una vuelta recorre la circunferencia $2\pi r$. Si tarda $T$, la rapidez es distancia dividida por tiempo:

$$
v_{\text{orb}}=\frac{2\pi r}{T}.
$$

Al sustituir esta rapidez en la ecuación orbital se obtiene

$$
\left(\frac{2\pi r}{T}\right)^2=\frac{GM}{r}
\quad\Longrightarrow\quad
T=2\pi\sqrt{\frac{r^3}{GM}}.
$$

La derivación muestra por qué un radio orbital mayor implica una rapidez circular menor y un período mayor. Ambas conclusiones dependen de que la órbita sea circular y de que la gravedad del cuerpo central domine.

## 6. Energía potencial gravitatoria: de dónde sale el signo negativo

La gravedad disminuye al alejarse: no es correcto suponer que su magnitud es constante para cualquier cambio de altura. Para hallar la energía potencial en el caso general usamos que la fuerza gravitatoria es conservativa: el trabajo entre dos radios depende solo del punto inicial y final, no de la trayectoria.

Definimos $r$ como la distancia al centro y elegimos positivo el sentido radial hacia afuera. Como la fuerza apunta hacia el centro, su componente radial es negativa:

$$
F_r=-\frac{GMm}{r^2}.
$$

El trabajo de la gravedad al mover el objeto desde $r_1$ hasta $r_2$ es

$$
W_{\text{grav},1\to2}
=\int_{r_1}^{r_2}F_r\,dr
=GMm\left(\frac{1}{r_2}-\frac{1}{r_1}\right).
$$

El cambio de energía potencial se define como el opuesto del trabajo gravitatorio:

$$
\Delta U=U_2-U_1=-W_{\text{grav},1\to2}.
$$

Tomemos el punto inicial en $r_1$ y el final a distancia $r$; luego hacemos que $r_1$ tienda al infinito:

$$
W_{\text{grav},r_1\to r}
=GMm\left(\frac{1}{r}-\frac{1}{r_1}\right)
\xrightarrow{r_1\to\infty}\frac{GMm}{r},
\qquad
U(r)-U(\infty)
=-\lim_{r_1\to\infty}W_{\text{grav},r_1\to r}
=-\frac{GMm}{r}.
$$

Al elegir $U(\infty)=0$, resulta

$$
U(r)=-\frac{GMm}{r}.
$$

El signo negativo indica que el objeto y el planeta forman un sistema ligado: con esta referencia, acercarlos reduce la energía potencial. Al alejar el objeto, la energía potencial aumenta y se acerca a cero. El cero es una elección de referencia; las diferencias de energía potencial son las que determinan el trabajo y el movimiento.

> [!warning] La fuerza y la energía potencial no tienen la misma dependencia con la distancia
> El módulo de la fuerza cambia como $1/r^2$. La energía potencial cambia como $-1/r$. La energía potencial se obtiene acumulando el trabajo de la fuerza a lo largo de un desplazamiento; no se copia la fórmula de la fuerza cambiándole el nombre.

### Cómo se recupera $mgh$ cerca de la superficie

Entre la superficie, en $R$, y una altura $h$, el cambio exacto de energía potencial es

$$
\Delta U
=U(R+h)-U(R)
=GMm\left(\frac{1}{R}-\frac{1}{R+h}\right)
=\frac{GMm\,h}{R(R+h)}.
$$

Si $h\ll R$, entonces $R+h\approx R$ en el denominador. Además, $g_0=GM/R^2$, por lo que

$$
\Delta U\approx\frac{GMm\,h}{R^2}=m g_0 h.
$$

Así se obtiene la fórmula conocida $mgh$: es una aproximación local de la expresión más general, válida cuando el campo cambia muy poco durante el desplazamiento.

## 7. Energía de una órbita y rapidez de escape

### Energía total en una órbita circular

La energía mecánica es la suma de la cinética y la potencial:

$$
E=K+U.
$$

En una órbita circular, la relación $v_{\text{orb}}^2=GM/r$ permite escribir

$$
K=\frac12mv_{\text{orb}}^2=\frac{GMm}{2r},
\qquad
U=-\frac{GMm}{r}.
$$

Al sumarlas,

$$
E_{\text{orb}}=-\frac{GMm}{2r}.
$$

El valor negativo indica que el satélite está ligado al planeta bajo la referencia $U(\infty)=0$. Para llegar al infinito y quedar allí en reposo, su energía total debe aumentar hasta cero.

### Rapidez mínima para escapar desde un radio dado

Imaginemos que un objeto se encuentra a distancia $r$ del centro y recibe una rapidez inicial $v_{\text{esc}}$. En el caso límite de escape, llega muy lejos con rapidez final cero. En el infinito tomamos $U_f=0$, así que su energía final es cero. Conservando la energía mecánica:

$$
\frac12m v_{\text{esc}}^2-\frac{GMm}{r}=0
\quad\Longrightarrow\quad
v_{\text{esc}}=\sqrt{\frac{2GM}{r}}.
$$

Esta rapidez es la **rapidez total** que debe tener en ese radio si se parte del caso definido en la derivación. No es automáticamente el aumento de rapidez que necesita un satélite que ya se mueve.

> [!example] Si el enunciado pregunta por la energía para escapar desde una órbita circular
> El satélite ya tiene energía inicial $E_i=-GMm/(2r)$. El estado límite de escape tiene $E_f=0$. Por lo tanto, la energía que hay que agregar es
>
> $$
> \Delta E=E_f-E_i=\frac{GMm}{2r}.
> $$
>
> Esta diferencia de energía no se calcula como si el satélite comenzara en reposo. Primero identifica el estado inicial que describe el problema; después compara su energía con la energía final de escape.

## 8. Kepler: del patrón observado a la relación de períodos

Kepler encontró sus leyes al analizar observaciones precisas de las posiciones planetarias. Sus relaciones describían los movimientos, aunque él no conocía la causa de la gravitación. Más tarde, Newton mostró cómo obtener esas leyes a partir del movimiento y de la gravitación. Para el parcial interesa especialmente la tercera ley: relaciona el período orbital con el tamaño de la órbita.

Para una órbita circular, ya tenemos dos relaciones:

$$
v=\frac{2\pi r}{T}
\qquad\text{y}\qquad
v^2=\frac{GM}{r}.
$$

La primera dice que rapidez es distancia recorrida por unidad de tiempo; la segunda viene de igualar la gravedad con la fuerza radial neta. Al combinarlas:

$$
\frac{4\pi^2r^2}{T^2}=\frac{GM}{r}
\quad\Longrightarrow\quad
T^2=\frac{4\pi^2}{GM}r^3.
$$

Para comparar dos cuerpos que orbitan la **misma masa central**, el factor $4\pi^2/(GM)$ es idéntico y se cancela:

$$
\frac{T_1^2}{r_1^3}=\frac{T_2^2}{r_2^3}.
$$

Esta es la forma útil para comparar, por ejemplo, la órbita de Marte con la de la Tierra alrededor del Sol. Las distancias pueden estar en cualquier unidad común si aparecen en un cociente; los períodos también deben estar en una misma unidad.

Para órbitas elípticas, el tamaño relevante es el **semieje mayor** $a$, la mitad del eje más largo de la elipse; en la relación de Kepler se usa $a$ donde en la órbita circular usamos $r$. En un círculo, $a=r$. En estos ejercicios, la masa orbitante se considera pequeña frente a la masa central. Si las dos masas fueran comparables, habría que describir el movimiento de ambas alrededor de su centro de masa e incluir las dos masas en la relación.

> [!warning] Cuándo no cancelar la constante
> Si los dos cuerpos orbitan masas centrales distintas, $GM$ no es el mismo y no se cancela. Antes de usar una razón de Kepler, verifica que ambos períodos y tamaños correspondan al mismo centro de atracción.

## Mapa: qué idea usar en cada tipo de pregunta

| Si el enunciado pide… | Empieza por… | Razón física |
|---|---|---|
| Fuerza entre dos masas | $F_g=GMm/r^2$ y dirección hacia la otra masa | Es la ley de interacción entre dos fuentes. |
| Campo o aceleración debida a varias masas | Calcular cada campo y sumarlo por componentes | La gravedad de varias fuentes se superpone vectorialmente. |
| Peso a distinta altura | $r=R+h$, luego comparar $g$ o $W$ | La ley usa distancia al centro. |
| Lectura de balanza en el ecuador | Segunda ley radial: $mg-N=ma_c$ | La persona necesita aceleración centrípeta. |
| Rapidez o período circular | Igualar gravedad con el requerimiento centrípeto | La gravedad curva la trayectoria. |
| Cambio de energía al subir mucho | $\Delta U=-W_{\text{grav}}$ | La fuerza cambia con la distancia; se integra su trabajo. |
| Energía para escapar desde una órbita | Comparar la energía orbital inicial con cero | El estado final límite en el infinito tiene energía total cero. |
| Comparación de períodos | Tercera ley de Kepler, con un mismo centro | Solo entonces la constante asociada a la masa central se cancela. |

## Secuencia sugerida

1. Lee las secciones 0–3 y explica con tus palabras la diferencia entre fuerza, campo y peso.
2. Repasa la caída libre y la órbita circular en las secciones 4–5.
3. Sigue el signo de $W_{\text{grav}}$ y $\Delta U$ en las secciones 6–7.
4. Estudia [[Teoría/01 - Fórmulas aplicadas de gravitación y órbitas]] y anota junto a cada fórmula qué supuesto la permite.
5. Resuelve [[Ejercicios/01 - Gravitación y órbitas]] sin abrir las pistas.
6. Compara con [[Resoluciones/01 - Gravitación y órbitas]] y registra qué decisión física te costó tomar.

## Fuentes consultadas

- [Capítulo 12, Gravitación](zotero://select/library/items/ATATDN6I): ley universal, acción y reacción, simetría esférica y superposición, PDF pp. 2–5 (libro pp. 384–387); campo, peso y variación con la distancia, PDF pp. 6–8 (pp. 388–390); trabajo, energía potencial, aproximación $mgh$ y escape, PDF pp. 8–11 (pp. 390–393); caída libre orbital, rapidez y período, PDF pp. 11–13 (pp. 393–395); leyes de Kepler, PDF pp. 15–17 (pp. 397–399).
- [TP 5: Gravitación, Física Aplicada 2025](zotero://select/library/items/F4BGIQ83), pp. 1–3: superposición, peso en distintos planetas y alturas, gravedad superficial, rotación, Kepler, satélites y energía.
- [Modelo del segundo parcial, Tema A, 11/11/2025](zotero://select/library/items/6GRRT3TK), pp. 1–2 escaneadas: aceleración por dos masas, satélite lunar y formulario entregado.

La guía explica y reorganiza esas ideas para estudiar; no es una transcripción literal del texto fuente.

## Autoevaluación de conceptos

Responde con tus palabras y escribe la relación física que respalda cada respuesta. Abre la explicación plegable solo después de intentarlo.

**1. Si la distancia entre dos masas se duplica, ¿por qué la fuerza queda en la cuarta parte? ¿Desde dónde se mide esa distancia?**

> [!success]- Mostrar explicación
> La ley universal dice $F_g\propto1/r^2$. Al reemplazar $r$ por $2r$, queda $F'_g/F_g=r^2/(2r)^2=1/4$. En planetas y otros cuerpos esféricamente simétricos vistos desde fuera, $r$ se mide entre los centros, no desde la superficie.

**2. ¿Por qué el campo de una fuente no depende del objeto de prueba y cómo se relaciona con su aceleración?**

> [!success]- Mostrar explicación
> Se define $\vec g=\vec F_g/m$. Al sustituir $\vec F_g=-GMm\,\hat{\mathbf r}/r^2$, la masa de prueba se cancela y queda $\vec g=-GM\,\hat{\mathbf r}/r^2$. Si no actúan otras fuerzas, $\vec a=\vec F_g/m=\vec g$. Las fuerzas sobre dos masas de prueba pueden ser distintas porque $F_g=mg$, aunque su aceleración gravitatoria sea la misma.

**3. Un objeto está a una altura igual al radio del planeta. ¿Qué distancia al centro usas y qué fracción del campo superficial tiene?**

> [!success]- Mostrar explicación
> Se usa $r=R+h=2R$. Como $g=GM/r^2$, su razón respecto del campo superficial es $g/g_0=(R/2R)^2=1/4$. La altura es la distancia sobre la superficie; la ley requiere la distancia desde el centro.

**4. ¿Qué dos ideas se combinan para obtener la rapidez orbital circular?**

> [!success]- Mostrar explicación
> La segunda ley de Newton requiere una fuerza neta radial $ma_c=mv^2/r$. En una órbita circular ideal, la gravedad es esa fuerza: $GMm/r^2=mv^2/r$. Al cancelar $m$ queda $v=\sqrt{GM/r}$. La dirección de la velocidad es tangente, mientras la aceleración apunta hacia el centro.

**5. ¿Por qué la energía potencial es negativa y en qué situación se recupera $mgh$?**

> [!success]- Mostrar explicación
> Se elige $U=0$ en el infinito. Al acercar dos masas, la gravedad realiza trabajo positivo y la energía potencial disminuye, por eso $U=-GMm/r<0$. Cerca de la superficie, si $h\ll R$, el cambio exacto $GMm(1/R-1/(R+h))$ se aproxima por $GMmh/R^2=mgh$, usando $g=GM/R^2$.

**6. ¿Cómo cambia el cálculo de energía de escape si el satélite ya está en una órbita circular?**

> [!success]- Mostrar explicación
> Desde el reposo a radio $r$, se impone energía final cero para obtener $v_{\text{esc}}=\sqrt{2GM/r}$. En una órbita circular el satélite ya tiene $E_i=-GMm/(2r)$. El incremento de energía requerido para llegar a cero es $\Delta E=GMm/(2r)$. Una rapidez de escape y una energía agregada son magnitudes distintas; el estado inicial determina cuál ecuación corresponde.

**7. ¿Cuándo se puede cancelar la constante de la tercera ley al comparar dos órbitas?**

> [!success]- Mostrar explicación
> Cuando ambos cuerpos orbitan la misma masa central y se mantiene el mismo modelo para las órbitas. En ese caso $4\pi^2/(GM)$ es común, de modo que $T_1^2/r_1^3=T_2^2/r_2^3$ (o se usan los semiejes mayores para órbitas elípticas). Si las masas centrales son distintas, el factor no es común.

**8. ¿Por qué la velocidad en una circunferencia es tangente, cómo se obtiene $v_t=2\pi r/T$ y de dónde sale $a_c=v_t^2/r$?**

> [!success]- Mostrar explicación
> En un intervalo muy corto, el desplazamiento entre dos posiciones se aproxima a la tangente; por eso la velocidad instantánea es tangente y perpendicular al radio. Una vuelta recorre $2\pi r$ durante un período $T$, así que $v_t=2\pi r/T$ (para movimiento uniforme). Entre dos instantes cercanos, las velocidades tienen módulo $v_t$ y difieren en un ángulo $\Delta\theta$: $|\Delta\vec v|\approx v_t\Delta\theta$. Como el arco cumple $\Delta s\approx r\Delta\theta$ y $v_t=\lim_{\Delta t\to0}\Delta s/\Delta t$, entonces $a_c=\lim_{\Delta t\to0}|\Delta\vec v|/\Delta t=v_t^2/r$, dirigida hacia el centro.

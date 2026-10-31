---
tags: [fisica-aplicada, teoria, conceptos, ondas-em]
---

# Conceptos de ondas electromagnéticas

[[Teoría/04 - Ondas electromagnéticas|← Índice del módulo]] · [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|Formulario aplicado]]

> [!summary] Idea central
> Una onda electromagnética es una perturbación que transporta energía mediante campos eléctrico y magnético variables. En el vacío, las leyes de Maxwell hacen que estos campos se relacionen y que la perturbación avance a $c$, sin necesitar un medio material.

## 1. Qué se propaga y qué oscila

En una onda sonora, las partículas del aire se desplazan un poco alrededor de sus posiciones de equilibrio. La perturbación pasa de una región a la siguiente porque las partículas interactúan. Si no hay medio, no hay sonido.

En una onda electromagnética no hace falta que se desplacen partículas de materia: lo que cambia de un lugar a otro son los campos eléctrico $\vec E$ y magnético $\vec B$. La luz visible, las ondas de radio, las microondas y los rayos X son miembros de la misma familia. Se distinguen principalmente por su frecuencia $f$ y su longitud de onda $\lambda$.

Un campo constante y uno variable se comportan de modo distinto. En electrostática y magnetostática se pueden estudiar campos que no cambian en el tiempo por separado. Cuando los campos cambian, las leyes de Faraday y Ampère-Maxwell los vinculan: la variación de uno está asociada con la circulación espacial del otro. Esa conexión permite que una perturbación electromagnética viaje por regiones donde no hay cargas ni corrientes.

## 2. Qué dicen las ecuaciones de Maxwell

La presentación del curso muestra las cuatro leyes en forma integral. La imagen reproduce esa diapositiva; la integral representa el flujo a través de una superficie cerrada o la circulación alrededor de una curva.

![[imagenes/maxwell-ecuaciones-presentacion.png]]

*Presentación de Ondas Electromagnéticas, diapositiva 5 (Zotero).*

> [!example]- Ver las cuatro leyes en forma integral
> $$
> \begin{aligned}
> \int_S \vec E\cdot d\vec A&=\frac{Q_{enc}}{\epsilon_0}
> &&\text{(Gauss eléctrica)},\\
> \int_S \vec B\cdot d\vec A&=0
> &&\text{(Gauss magnética)},\\
> \oint_C \vec E\cdot d\vec\ell&=-\frac{d\Phi_B}{dt}
> &&\text{(Faraday)},\\
> \oint_C \vec B\cdot d\vec\ell&=\mu_0\left(I_{enc}+\epsilon_0\frac{d\Phi_E}{dt}\right)
> &&\text{(Ampère-Maxwell)}.
> \end{aligned}
> $$
>
> $S$ es una superficie cerrada y $C$ su borde; $d\vec A$ y $d\vec\ell$ son pequeños elementos orientados de área y de recorrido. El flujo mide cuánto campo atraviesa una superficie: $\Phi_E=\int\vec E\cdot d\vec A$ y $\Phi_B=\int\vec B\cdot d\vec A$. La circulación suma la componente del campo a lo largo de un recorrido cerrado. En el vacío sin cargas ni corrientes de conducción, $Q_{enc}=0$ e $I_{enc}=0$, pero el flujo eléctrico puede variar; ese último término es el aporte de Maxwell.

En palabras:

1. **Ley de Gauss eléctrica:** la carga eléctrica encerrada es fuente o sumidero del campo eléctrico.
2. **Ley de Gauss magnética:** el flujo magnético neto a través de una superficie cerrada es cero; no se han observado cargas magnéticas aisladas.
3. **Ley de Faraday:** un flujo magnético que cambia induce circulación de campo eléctrico. El signo menos expresa la orientación de esa inducción.
4. **Ley de Ampère-Maxwell:** una corriente eléctrica o un flujo eléctrico variable induce circulación de campo magnético. El término de Maxwell, proporcional a la variación del flujo eléctrico, es crucial incluso donde no circula corriente material.

Para una onda que se propaga en el vacío lejos de cargas y corrientes, las leyes locales se simplifican a

$$
\begin{aligned}
\nabla\cdot\vec E&=0, & \nabla\cdot\vec B&=0,\\
\nabla\times\vec E&=-\frac{\partial\vec B}{\partial t}, &
\nabla\times\vec B&=\mu_0\epsilon_0\frac{\partial\vec E}{\partial t}.
\end{aligned}
$$

Aquí $\nabla\cdot$ describe si un campo sale netamente de una pequeña región; $\nabla\times$ describe su circulación local. No hace falta calcular estos operadores en los ejercicios del módulo: las ecuaciones ayudan a entender por qué las fórmulas funcionan.

> [!note] Qué aporta el término de Maxwell
> En la expresión de Ampère aparece $\epsilon_0\,\partial\vec E/\partial t$. Si se lo omitiera, una onda en el vacío no podría mantener la relación entre los campos variables. Maxwell añadió este término para que la ley fuera consistente cuando cambia el campo eléctrico, incluso en una región sin corriente de conducción.

## 3. Por qué aparece una ecuación de onda

Las dos leyes de circulación muestran el vínculo local: un $\vec B$ que cambia está acompañado por circulación de $\vec E$, y un $\vec E$ que cambia está acompañado por circulación de $\vec B$. Al combinar esas relaciones, cada campo satisface una ecuación de onda:

$$
\nabla^2\vec E-\mu_0\epsilon_0\frac{\partial^2\vec E}{\partial t^2}=0,
\qquad
\nabla^2\vec B-\mu_0\epsilon_0\frac{\partial^2\vec B}{\partial t^2}=0.
$$

La estructura coincide con la ecuación general de una onda que viaja a rapidez $v$,

$$
\nabla^2\psi-\frac{1}{v^2}\frac{\partial^2\psi}{\partial t^2}=0.
$$

Al comparar los coeficientes se obtiene

$$
v=\frac{1}{\sqrt{\mu_0\epsilon_0}}=c\approx3.00\times10^8\,\mathrm{m/s}.
$$

La constante $\epsilon_0$ es la permitividad eléctrica del vacío y $\mu_0$ su permeabilidad magnética. En las ecuaciones de Maxwell conectan cuánto cambia cada campo con el otro; por eso su producto fija la rapidez de propagación.

Así se entiende el resultado central de Maxwell: las ecuaciones del electromagnetismo predicen una onda que viaja a la rapidez de la luz. La luz es una onda electromagnética.

> [!example]- Desglose matemático opcional: de Faraday a la ecuación de onda
> En el vacío, $\nabla\cdot\vec E=0$ y $\nabla\times\vec E=-\partial\vec B/\partial t$. Aplicamos rotacional a ambos lados de la ley de Faraday y sustituimos $\nabla\times\vec B=\mu_0\epsilon_0\,\partial\vec E/\partial t$:
>
> $$
> \nabla\times(\nabla\times\vec E)
> =-\frac{\partial}{\partial t}(\nabla\times\vec B)
> =-\mu_0\epsilon_0\frac{\partial^2\vec E}{\partial t^2}.
> $$
>
> Se usa la identidad $\nabla\times(\nabla\times\vec E)=\nabla(\nabla\cdot\vec E)-\nabla^2\vec E$. Como $\nabla\cdot\vec E=0$, queda $-\nabla^2\vec E=-\mu_0\epsilon_0\,\partial^2\vec E/\partial t^2$. Al cancelar los signos menos resulta la ecuación de onda eléctrica. El mismo procedimiento, intercambiando los papeles de $\vec E$ y $\vec B$, conduce a la ecuación magnética.

## 4. Geometría: los campos son transversales

Para una onda plana que avanza en la dirección $\hat n$, los campos oscilan en direcciones perpendiculares al avance y entre sí:

$$
\vec E\perp\vec B,\qquad
\vec E\perp\hat n,\qquad
\vec B\perp\hat n.
$$

Por eso la onda es **transversal**. La dirección de avance no es la dirección hacia la que apunta $\vec E$ ni $\vec B$: es perpendicular a ambas.

La relación vectorial entre las direcciones es

$$
\vec B=\frac{1}{c}\,\hat n\times\vec E,
\qquad
\vec E\times\vec B\ \text{apunta como}\ \hat n.
$$

La primera forma sirve para encontrar $\vec B$ una vez elegidos el avance y $\vec E$; la segunda es un control de signo. El orden del producto vectorial importa: invertir los factores invierte la dirección.

![[imagenes/onda-electromagnetica.svg]]

> [!example]- ¿Por qué los campos son perpendiculares al avance?
> En una región sin carga, $\nabla\cdot\vec E=0$. Para una onda plana, la variación espacial ocurre en la dirección de su vector de onda $\vec k$; al aplicar la divergencia, esta condición implica $\vec k\cdot\vec E_{max}=0$. Por tanto, $\vec E$ es perpendicular a la propagación. El mismo razonamiento con $\nabla\cdot\vec B=0$ muestra que $\vec B$ también es transversal. La ley de Faraday fija además la orientación relativa entre ambos.

## 5. Cómo se relacionan las magnitudes de $\vec E$ y $\vec B$

En una solución sinusoidal plana en el vacío, las ecuaciones de Maxwell obligan a que ambos campos compartan la fase: alcanzan sus máximos, mínimos y cruces por cero en los mismos puntos y momentos. Sus amplitudes sí tienen unidades diferentes, pero están ligadas por

$$
E_{max}=cB_{max},\qquad B_{max}=\frac{E_{max}}{c}.
$$

La rapidez $c$ hace que la ecuación sea dimensionalmente consistente: $(\mathrm{m/s})(\mathrm T)=\mathrm{V/m}$. No se afirma que los dos valores numéricos sean iguales.

El origen de esta relación se desarrolla paso a paso en [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|el formulario aplicado]]. En síntesis, la ley de Faraday conecta la variación espacial de $\vec E$ con la variación temporal de $\vec B$; para una onda sinusoidal, esto da $kE_{max}=\omega B_{max}$. Como $\omega/k=c$ en el vacío, resulta $E_{max}/B_{max}=c$.

## 6. Frecuencia, longitud de onda y rapidez

La frecuencia $f$ cuenta cuántos ciclos pasan por un punto cada segundo. El período $T=1/f$ es el tiempo que tarda un ciclo. La longitud de onda $\lambda$ es la distancia entre dos puntos vecinos que están en la misma fase.

Durante un período, el patrón avanza una longitud de onda. Por definición de rapidez:

$$
v=\frac{\lambda}{T}=\lambda f.
$$

En el vacío $v=c$, por lo que

$$
c=\lambda f,\qquad f=\frac{c}{\lambda},\qquad \lambda=\frac{c}{f}.
$$

La fuente fija la frecuencia. Si $f$ aumenta y la propagación sigue siendo en el vacío, $\lambda$ disminuye para que el producto $\lambda f$ siga siendo $c$. En los ejercicios de este módulo se usa el vacío; no reemplaces $c$ por una rapidez de otro medio sin que el problema lo indique.

## 7. Fase: cómo leer el sentido de propagación

Una onda sinusoidal puede escribirse mediante la fase

$$
\Phi(x,t)=kx-\omega t+\phi_0,
$$

donde $k=2\pi/\lambda$ mide el cambio de fase por distancia, $\omega=2\pi f$ mide el cambio de fase por tiempo y $\phi_0$ fija la fase inicial.

Para saber hacia dónde avanza una forma de onda, sigue una cresta manteniendo su fase constante. Si $kx-\omega t=C$,

$$
\frac{dx}{dt}=+\frac{\omega}{k};
$$

la cresta se mueve hacia $+x$. Si la fase es $kx+\omega t=C$, entonces $dx/dt=-\omega/k$ y se mueve hacia $-x$.

![[imagenes/sentido-fase-onda.svg]]

## 8. Energía que transporta la onda

Los campos almacenan energía eléctrica y magnética, y la onda la transporta por el espacio. La dirección del flujo de energía se representa mediante el vector de Poynting:

$$
\vec S=\frac{1}{\mu_0}\,\vec E\times\vec B.
$$

Su unidad es $\mathrm{W/m^2}$. En una onda sinusoidal, $\vec E$ y $\vec B$ cambian de signo juntos, así que su producto mantiene el sentido de propagación. Para una onda plana, el valor medio es $\langle S\rangle=E_{max}B_{max}/(2\mu_0)$. Esta idea explica por qué decimos que la onda transporta energía: los ejercicios 20–21 se centran en las amplitudes y direcciones, mientras que C24–C27 practican los cálculos de densidad, flujo e intensidad media.

La densidad de energía en el vacío suma lo almacenado en ambos campos:

$$
u=\frac12\epsilon_0E^2+\frac{B^2}{2\mu_0}.
$$

Como para una onda plana $E=cB$, cada término aporta lo mismo y $u=\epsilon_0E^2$. El vector de Poynting indica cuánta energía cruza por unidad de área y tiempo; para una onda progresiva en el vacío, $S=cu$. Si los campos forman una sinusoide, el valor medio incluye un factor $1/2$ porque $\langle\cos^2\rangle=1/2$. Un pulso de frente plano con campos constantes detrás de su frente se resuelve con los valores instantáneos, sin ese promedio.

### Cuando la onda entra a un material

La onda sigue siendo electromagnética, pero el material responde al campo y modifica su rapidez. En un material lineal, uniforme y sin pérdidas, con permitividad $\epsilon=K\epsilon_0$ y permeabilidad $\mu=K_m\mu_0$,

$$
v=\frac{1}{\sqrt{\epsilon\mu}}=\frac{c}{\sqrt{KK_m}}.
$$

La frecuencia se conserva al cruzar una superficie estacionaria porque la fuente sigue oscilando al mismo ritmo a ambos lados. Como $v=\lambda f$, si baja la rapidez dentro del material, también baja la longitud de onda. Por eso para hallar la longitud de onda en el medio se usa $\lambda=v/f$; $c/f$ solo da la longitud de onda en el vacío. La relación entre rapidez, permitividad y permeabilidad se desarrolla en [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas#6. Rapidez y longitud de onda dentro de un material]].

### La onda también transfiere momento

La luz puede ejercer una fuerza porque transporta momento junto con energía. Si incide perpendicularmente sobre un panel que absorbe la radiación, el momento incidente queda en el panel y la presión media es $p_{rad}=I/c$. Si la luz se refleja perfectamente, su momento cambia de sentido y la transferencia se duplica: $p_{rad}=2I/c$. Una vez conocida la presión, la fuerza es $F=p_{rad}A$.

### Ondas estacionarias: campos presentes, flujo medio nulo

Al superponer dos ondas de igual frecuencia que viajan en direcciones opuestas se forman nodos fijos. En una onda estacionaria ideal, la energía fluye momentáneamente hacia adelante y hacia atrás; al promediar un período, el flujo neto en cada posición es cero. Esto no significa que $\vec E$ y $\vec B$ sean siempre cero: sus amplitudes espaciales tienen nodos y máximos en lugares distintos.

Entre paredes conductoras, el campo eléctrico tangencial debe anularse en las superficies. Para que la onda estacionaria satisfaga esa condición en ambas paredes, la distancia $L$ debe incluir un número entero de medias longitudes de onda, $L=m\lambda/2$. En el modo fundamental cabe media longitud de onda: $\lambda_1=2L$. El campo eléctrico tiene un nodo en cada pared y un máximo en el centro; el campo magnético presenta el patrón complementario. Las condiciones de modo se resumen en [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas#10. Modos estacionarios en una cavidad]].

## 9. De la descripción física a las ecuaciones de campo

Para construir $\vec E(x,t)$ y $\vec B(x,t)$, toma las decisiones en este orden:

1. Dibuja los ejes e identifica el vector unitario de propagación $\hat n$.
2. Anota la amplitud y el sentido de $\vec E$ que da el problema. Si solo da su magnitud, declara una orientación conveniente.
3. Encuentra la amplitud que falta con $E_{max}=cB_{max}$ o $B_{max}=E_{max}/c$.
4. Determina $\vec B$ con $\hat n\times\vec E$ y comprueba que $\vec E\times\vec B$ apunta como $\hat n$.
5. Elige una fase que viaje en el sentido correcto: $kx-\omega t$ para $+x$, $kx+\omega t$ para $-x$.
6. Usa la misma fase en ambos campos y verifica sus unidades.

Las amplitudes vectoriales contienen sentido y magnitud; por ejemplo, $\vec E_{max}=E_{max}\hat y$. No escondas un signo negativo tanto en el vector como en la fase: eso puede invertir dos veces el sentido.

## Errores que conviene evitar

- Confundir la orientación de un campo con la dirección en que avanza la onda.
- Pensar que una onda electromagnética necesita aire o que transporta materia desde la fuente.
- Usar $c=\lambda f$ en un medio material sin comprobar cuál es la rapidez indicada.
- Confundir $f$ (ciclos por segundo) con $\omega$ (radianes por segundo), o $1/\lambda$ con $k=2\pi/\lambda$.
- Usar $E_{max}=cB_{max}$ sin convertir militeslas a teslas.
- Elegir el sentido de $\vec B$ a ojo; comprueba el producto vectorial.
- Cambiar el signo de la fase sin cambiar el sentido físico de propagación.

## Fuentes de esta nota

La [presentación de Ondas Electromagnéticas](zotero://select/library/items/FQBGWVB4), diapositivas 2–5, presenta la diferencia entre ondas mecánicas y electromagnéticas, la relación entre campos variables, las cuatro leyes de Maxwell y su aplicación en el vacío. Se revisaron visualmente las diapositivas 4–5 para interpretar sus ecuaciones integrales. La [práctica de ondas electromagnéticas](zotero://select/library/items/T92A4S8A), PDF pp. 2–9, incluye ecuaciones vectoriales, propagación en medios, energía y flujo, presión de radiación, ondas estacionarias y modos de cavidad. Véase [[Fuentes Zotero y probabilidad]].

## Autoevaluación de conceptos

Responde sin abrir la explicación; luego identifica qué idea física te permitió contestar.

**1. ¿Qué se desplaza en una onda electromagnética y qué diferencia principal tiene con el sonido?**

> [!success]- Mostrar explicación
> En la onda electromagnética varían los campos $\vec E$ y $\vec B$; no es necesario que las partículas de un medio oscilen. El sonido sí es una perturbación mecánica y necesita un medio material cuyas partículas transmitan la perturbación.

**2. ¿Qué relación establecen Faraday y Ampère-Maxwell cuando los campos cambian en el tiempo?**

> [!success]- Mostrar explicación
> Un campo magnético variable está asociado con circulación de campo eléctrico; un campo eléctrico variable está asociado con circulación de campo magnético. Juntas, estas leyes permiten que la perturbación se propague aun donde no hay materia, carga ni corriente de conducción.

**3. ¿De dónde sale la rapidez $c$ en la ecuación de onda electromagnética?**

> [!success]- Mostrar explicación
> Al combinar las leyes de Maxwell en el vacío se obtiene una ecuación de onda cuyo coeficiente temporal es $\mu_0\epsilon_0$. Al compararla con la ecuación general de onda, la rapidez es $1/\sqrt{\mu_0\epsilon_0}$, que coincide con la rapidez de la luz.

**4. Si la onda avanza hacia $+x$ y $\vec E$ apunta en $+y$, ¿cómo determinas $\vec B$?**

> [!success]- Mostrar explicación
> Usa $\vec B=(1/c)\hat n\times\vec E$. Como $\hat x\times\hat y=\hat z$, $\vec B$ apunta en $+z$. Comprueba que $\vec E\times\vec B$ quede en $+x$.

**5. ¿Por qué en el vacío una frecuencia mayor implica una longitud de onda menor?**

> [!success]- Mostrar explicación
> La rapidez es constante e igual a $c$, y $c=\lambda f$. Si $f$ aumenta, $\lambda$ debe disminuir para mantener constante el producto. La frecuencia la fija la fuente; la longitud de onda acompaña la rapidez de propagación.

**6. ¿Cómo decides si la fase es $kx-\omega t$ o $kx+\omega t$?**

> [!success]- Mostrar explicación
> Mantén constante la fase para seguir una cresta. $kx-\omega t=C$ implica $dx/dt=+\omega/k$ y avance hacia $+x$; $kx+\omega t=C$ implica $dx/dt=-\omega/k$ y avance hacia $-x$.

**7. Una onda pasa del vacío a un material. Si la frecuencia se conserva y la rapidez baja, ¿qué le pasa a la longitud de onda?**

> [!success]- Mostrar explicación
> La relación $v=\lambda f$ debe cumplirse en el nuevo medio. Como $f$ sigue teniendo el valor que fija la fuente y $v$ es menor, $\lambda=v/f$ también es menor. El campo no cambia la frecuencia para acomodarse al material.

**8. ¿Por qué un pulso plano con campos constantes usa $S=EB/\mu_0$, mientras que para una onda sinusoidal se usa $I=E_{max}B_{max}/(2\mu_0)$?**

> [!success]- Mostrar explicación
> $S=EB/\mu_0$ es el flujo instantáneo. En un pulso con el valor indicado constante detrás del frente, esos campos son directamente los valores instantáneos. Para una sinusoide se busca el promedio de $S$ durante un ciclo; como el producto contiene $\cos^2$, su promedio es $1/2$, y se obtiene la fórmula con amplitudes máximas.

**9. ¿Qué cambia en la presión de radiación si una superficie absorbe la luz o la refleja perfectamente?**

> [!success]- Mostrar explicación
> La radiación incidente lleva momento. Si se absorbe, transfiere el momento incidente y $p_{rad}=I/c$. Si se refleja perfectamente, invierte el momento y el cambio transferido se duplica: $p_{rad}=2I/c$. Luego la fuerza es presión por área.

**10. En el modo fundamental de una cavidad, ¿por qué $E$ es nulo en las paredes y máximo en el centro? ¿Qué sucede con $B$?**

> [!success]- Mostrar explicación
> En las paredes conductoras la componente tangencial de $E$ debe ser cero; como las paredes son nodos consecutivos en el modo fundamental, hay media longitud de onda entre ellas y un antinodo de $E$ en el centro. La amplitud espacial de $B$ queda desplazada: alcanza máximos en las paredes y se anula en el centro. El flujo medio neto es cero aunque los campos oscilen.

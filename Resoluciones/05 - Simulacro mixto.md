---
tags: [fisica-aplicada, resoluciones, simulacro]
---

# Corrección paso a paso — simulacro mixto

Intenta cada problema antes de leer su solución. La meta es poder justificar la ecuación a partir del fenómeno y de los datos, además de obtener el número.

## Problema 1 — Campo gravitatorio por superposición

### 1. Interpretar posiciones y sentidos

El campo gravitatorio de una masa puntual siempre apunta hacia esa masa. Desde el origen:

- $M_1$ está al oeste, a $r_1=3.00\,\mathrm{km}=3.00\times10^3\,\mathrm{m}$; su campo apunta en $-x$.
- $M_2$ está al norte, a $r_2=4.00\,\mathrm{km}=4.00\times10^3\,\mathrm{m}$; su campo apunta en $+y$.

Por superposición, sumamos vectorialmente las contribuciones. Los kilómetros se convierten a metros porque $G$ está expresada en unidades SI.

### 2. Calcular cada contribución

Para una masa puntual, el módulo del campo es $g=GM/r^2$.

$$
g_1=\frac{(6.67\times10^{-11})(4.00\times10^{11})}{(3.00\times10^3)^2}
=2.964\times10^{-6}\,\mathrm{m/s^2}.
$$

$$
g_2=\frac{(6.67\times10^{-11})(9.00\times10^{11})}{(4.00\times10^3)^2}
=3.752\times10^{-6}\,\mathrm{m/s^2}.
$$

Al asignar los sentidos encontrados en el dibujo:

$$
\vec g_1=-2.964\times10^{-6}\,\hat x\,\mathrm{m/s^2},
\qquad
\vec g_2=+3.752\times10^{-6}\,\hat y\,\mathrm{m/s^2}.
$$

Por lo tanto,

$$
\vec g=(-2.964\,\hat x+3.752\,\hat y)\times10^{-6}\,\mathrm{m/s^2}.
$$

### 3. Módulo y dirección

Las componentes son perpendiculares, así que usamos Pitágoras:

$$
|\vec g|=\sqrt{g_x^2+g_y^2}
=\sqrt{(2.964\times10^{-6})^2+(3.752\times10^{-6})^2}
=4.782\times10^{-6}\,\mathrm{m/s^2}.
$$

El ángulo al norte del oeste se mide desde la dirección $-x$:

$$
\theta=\tan^{-1}\!\left(\frac{g_y}{|g_x|}\right)
=\tan^{-1}\!\left(\frac{3.752}{2.964}\right)
=51.7^\circ.
$$

El campo apunta $51.7^\circ$ al norte del oeste.

### 4. Fuerza sobre la masa de prueba

El campo describe la fuerza por unidad de masa; por eso no cambia al cambiar la masa de prueba. La fuerza sí depende de ella:

$$
\vec F=m\vec g
=(150\,\mathrm{kg})(-2.964\times10^{-6}\,\hat x
+3.752\times10^{-6}\,\hat y)\,\mathrm{m/s^2}.
$$

$$
\vec F=(-4.447\,\hat x+5.628\,\hat y)\times10^{-4}\,\mathrm N,
\qquad
|\vec F|=m|\vec g|=7.173\times10^{-4}\,\mathrm N.
$$

La fuerza tiene la misma dirección que el campo. Si se suelta la masa desde el reposo, su aceleración inicial es $\vec a=\vec F/m=\vec g$.

**Control:** el campo apunta hacia el noroeste, entre las dos masas que atraen; la unidad $\mathrm{N/kg}$ del campo equivale a $\mathrm{m/s^2}$.

## Problema 2 — Tiempo propio y longitud propia

### 1. Factor de Lorentz

La rapidez es $v=0.800c$, por lo tanto:

$$
\gamma=\frac{1}{\sqrt{1-v^2/c^2}}
=\frac{1}{\sqrt{1-0.800^2}}
=1.667.
$$

### 2. Intervalo temporal

Los dos destellos ocurren en el mismo punto de la nave. El reloj que acompaña a ese punto mide el tiempo propio $\Delta t_0=4.00\,\mathrm{años}$. Para la Tierra, los eventos ocurren en lugares diferentes y el intervalo es dilatado:

$$
\Delta t=\gamma\Delta t_0
=(1.667)(4.00\,\mathrm{años})
=6.67\,\mathrm{años}.
$$

La Tierra mide un intervalo mayor que el reloj que acompaña a los eventos, como predice la dilatación temporal.

### 3. Longitud medida desde la Tierra

$L_0=180\,\mathrm m$ es la longitud propia porque se mide en reposo respecto de la nave. La Tierra observa la nave en movimiento, así que mide una longitud contraída:

$$
L=\frac{L_0}{\gamma}
=\frac{180\,\mathrm m}{1.667}
=108\,\mathrm m.
$$

Para medir esa longitud, el observador terrestre debe registrar las posiciones de ambos extremos **al mismo tiempo en el marco de la Tierra**. Esta simultaneidad hace que la longitud corresponda al mismo instante terrestre.

**Control:** $\Delta t>\Delta t_0$ y $L<L_0$, de acuerdo con dilatación temporal y contracción de longitud.

## Problema 3 — Nivel sonoro y efecto Doppler

### a. Sumar dos fuentes independientes

El nivel de una fuente se relaciona con la intensidad mediante

$$
\beta_1=10\log_{10}\!\left(\frac{I_1}{I_0}\right).
$$

Despejamos antes de sustituir:

$$
I_1=I_0\,10^{\beta_1/10}
=(1.00\times10^{-12})10^{72.0/10}
=1.585\times10^{-5}\,\mathrm{W/m^2}.
$$

Las fuentes son independientes, por lo que sumamos sus intensidades:

$$
I_{\mathrm{tot}}=I_1+I_1=2I_1
=3.170\times10^{-5}\,\mathrm{W/m^2}.
$$

El nuevo nivel es

$$
\beta_{\mathrm{tot}}=10\log_{10}\!\left(\frac{I_{\mathrm{tot}}}{I_0}\right)
=75.01\,\mathrm{dB}.
$$

Duplicar la intensidad aumenta el nivel en

$$
\Delta\beta=10\log_{10}(2)=3.01\,\mathrm{dB}.
$$

No se duplican los decibeles porque la escala es logarítmica; primero se suman intensidades y luego se toma el logaritmo.

### b. Fuente y observador que se acercan

Para sonido con el medio en reposo, si fuente y observador se acercan:

$$
f_{\mathrm{obs}}=f_s\frac{v+v_o}{v-v_s}.
$$

El observador se acerca a los frentes y aumenta la rapidez con que los encuentra: por eso $v_o$ se suma. La fuente se acerca y emite frentes desde posiciones cada vez más próximas al observador: la longitud de onda frontal se acorta, lo que corresponde a restar $v_s$ en el denominador.

$$
f_{\mathrm{obs}}
=(600\,\mathrm{Hz})\frac{343+10.0}{343-25.0}
=(600)\frac{353}{318}\,\mathrm{Hz}
=666.0\,\mathrm{Hz}.
$$

La frecuencia recibida es mayor que la emitida, tal como corresponde a ambos movimientos de acercamiento.

**Control:** se usó la rapidez del sonido respecto del aire en el marco donde el aire está en reposo; las velocidades de fuente y observador son mucho menores que $v$.

## Problema 4 — Onda electromagnética en el vacío

### 1. Convertir y calcular magnitudes

Convertimos los datos:

$$
\lambda=20.0\,\mathrm{\mu m}=2.00\times10^{-5}\,\mathrm m,
\qquad
B_{\max}=1.80\,\mathrm{mT}=1.80\times10^{-3}\,\mathrm T.
$$

En el vacío, la onda se propaga a $c$, de modo que

$$
f=\frac{c}{\lambda}
=\frac{3.00\times10^8}{2.00\times10^{-5}}
=1.50\times10^{13}\,\mathrm{Hz}.
$$

La ley de Faraday y la ley de Ampère-Maxwell relacionan las variaciones de ambos campos. Para una onda plana en el vacío, sus amplitudes cumplen $E_{\max}=cB_{\max}$:

$$
E_{\max}=(3.00\times10^8)(1.80\times10^{-3})
=5.40\times10^5\,\mathrm{V/m}.
$$

El número de onda y la frecuencia angular son

$$
k=\frac{2\pi}{\lambda}
=3.14\times10^5\,\mathrm{rad/m},
\qquad
\omega=2\pi f
=9.42\times10^{13}\,\mathrm{rad/s}.
$$

### 2. Determinar la dirección de $\vec B$

La onda avanza en $+z$ y $\vec E_{\max}$ apunta en $+x$. Para que la energía avance en $+z$, los tres vectores deben satisfacer

$$
\vec B_{\max}=\frac{1}{c}\,\hat z\times\vec E_{\max}.
$$

Como $\hat z\times\hat x=\hat y$, el campo magnético apunta en $+y$.

### 3. Escribir las ecuaciones de campo

Una fase $kz-\omega t$ se desplaza hacia $+z$. Además, en $z=0,t=0$ el coseno vale 1, de modo que el campo eléctrico tiene el máximo positivo indicado. Por lo tanto,

$$
\vec E(z,t)=
(5.40\times10^5\,\mathrm{V/m})
\cos\!\left[(3.14\times10^5\,\mathrm{rad/m})z
-(9.42\times10^{13}\,\mathrm{rad/s})t\right]\hat x,
$$

$$
\vec B(z,t)=
(1.80\times10^{-3}\,\mathrm T)
\cos\!\left[(3.14\times10^5\,\mathrm{rad/m})z
-(9.42\times10^{13}\,\mathrm{rad/s})t\right]\hat y.
$$

### 4. Controles

Al mantener la fase constante, $kz-\omega t=\mathrm{constante}$, se obtiene $z=(\omega/k)t+\mathrm{constante}$: la fase avanza en $+z$. También,

$$
\vec E\times\vec B\propto\hat x\times\hat y=\hat z,
$$

así que la dirección de propagación coincide con la del flujo de energía.

**Control de amplitudes:** $E_{\max}/B_{\max}=5.40\times10^5/(1.80\times10^{-3})=3.00\times10^8\,\mathrm{m/s}=c$.

## Puntaje sugerido para autocorrección

En cada problema, asigna hasta 5 puntos por la representación y convenciones, 8 por escoger y justificar el modelo, 7 por el planteo y los cálculos, y 5 por unidades, dirección y control final. En el problema 3 reparte el puntaje entre sus dos apartados.

Registra los errores por categoría en [[Ejercicios/00 - Método y registro]] y repite desde cero los dos problemas donde haya fallado la elección del principio o del signo.

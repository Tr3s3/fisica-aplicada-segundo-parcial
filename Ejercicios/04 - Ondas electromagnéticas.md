---
tags: [fisica-aplicada, ejercicios, ondas-em]
---

# Ejercicios — Ondas electromagnéticas

**Conceptos:** [[Teoría/04 - Conceptos de ondas electromagnéticas]] · **Fórmulas:** [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas]] · **Resoluciones:** [[Resoluciones/04 - Ondas electromagnéticas]] · **Método:** [[Ejercicios/00 - Método y registro]]

> [!info] Cómo usar esta hoja
> Resuelve primero sin abrir la pista. **M** conserva el tipo y los datos centrales de un modelo de parcial. **R** ejercita transferencia con una situación de la práctica de Zotero. **C** cubre temas del TP que no aparecen en los modelos revisados. Las orientaciones añadidas se indican para que cada vector tenga un sentido único.

## Ejercicios del tema

### 20. De los datos de la onda a las ecuaciones vectoriales — **M**

**Situación.** El modelo 2024 da una onda electromagnética sinusoidal en el vacío con amplitud magnética $B_{max}=2.15\,\mathrm{mT}$ y longitud de onda $\lambda=350\,\mathrm{nm}$, y pide la frecuencia, la amplitud eléctrica y las ecuaciones de los campos. Para practicar la forma vectorial sin ambigüedad, fijamos además esta convención: la onda avanza en $+x$ y $\vec E$ apunta en $+y$.

**Datos**

- $\lambda=350\,\mathrm{nm}$.
- $B_{max}=2.15\,\mathrm{mT}$.
- $c=3.00\times10^8\,\mathrm{m/s}$.
- $\hat n=+\hat x$ y $\vec E_{max}$ apunta en $+\hat y$.

**Se pide**

1. Calcula $f$, $E_{max}$, $k$ y $\omega$.
2. Determina la dirección de $\vec B$.
3. Escribe $\vec E(x,t)$ y $\vec B(x,t)$.
4. Comprueba que $\vec E\times\vec B$ apunta en el sentido de propagación.

![[imagenes/onda-electromagnetica.svg]]

> [!tip]- Pista de arranque
>
> Convierte nm y mT a SI. Usa $f=c/\lambda$, $E_{max}=cB_{max}$, $k=2\pi/\lambda$ y $\omega=2\pi f$. Para el sentido, calcula $\hat n\times\vec E_{max}$ y revisa $\vec E_{max}\times\vec B_{max}$.

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 20]].

### 21. Onda láser que avanza hacia $-x$ — **R**

**Situación.** Un láser de dióxido de carbono emite en el vacío una onda sinusoidal que viaja hacia $-x$. Su longitud de onda es $10.6\,\mathrm{\mu m}$ y el campo eléctrico es paralelo al eje $z$, con amplitud $1.53\,\mathrm{MV/m}$. Para fijar la orientación vectorial, toma $\vec E_{max}$ en $+\hat z$.

**Datos**

- $\lambda=10.6\,\mathrm{\mu m}$.
- $E_{max}=1.53\,\mathrm{MV/m}$.
- $c=3.00\times10^8\,\mathrm{m/s}$.
- $\hat n=-\hat x$ y $\vec E_{max}$ apunta en $+\hat z$.

**Se pide**

1. Calcula $f$, $B_{max}$, $k$ y $\omega$.
2. Determina la dirección de $\vec B$ con el producto vectorial.
3. Escribe las ecuaciones vectoriales de ambos campos como función de $x$ y $t$.
4. Comprueba que la fase elegida representa avance hacia $-x$ y que $\vec E\times\vec B$ tiene el sentido correcto.

![[imagenes/sentido-fase-onda.svg]]

> [!tip]- Pista de arranque
>
> $10.6\,\mathrm{\mu m}=1.06\times10^{-5}\,\mathrm m$. Usa $B_{max}=E_{max}/c$, $k=2\pi/\lambda$ y $\omega=2\pi f$. Para avanzar hacia $-x$, prueba la fase $kx+\omega t$. Luego comprueba $+\hat z\times\hat y$.

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 21]].

## Ejercicios complementarios del TP

Estos ejercicios amplían la práctica más allá de la familia de ecuaciones vectoriales que aparece en el modelo. No son predicciones de examen: sirven para cubrir los otros contenidos de la unidad que sí están desarrollados en el TP.

### 22. Luz de sodio que atraviesa un diamante — **C · prioridad media**

Una lámpara de vapor de sodio emite luz amarilla de frecuencia $f=5.09\times10^{14}\,\mathrm{Hz}$. La luz pasa del aire al diamante. Para esta frecuencia, usa para el diamante la constante dieléctrica relativa $K=5.84$ y la permeabilidad relativa $K_m=1.00$. Trata el aire como vacío y desprecia pérdidas y reflexiones.

**Se pide.**

1. Calcula la longitud de onda en el aire/vacío.
2. Calcula la rapidez de propagación en el diamante.
3. Calcula la longitud de onda dentro del diamante.
4. Explica cuál de las magnitudes $f$, $v$ y $\lambda$ cambia al cruzar la superficie y por qué.

> [!tip]- Pista de planteo
> La rapidez en un medio lineal es $v=c/\sqrt{KK_m}$. La frecuencia la fija la fuente y se conserva al cruzar la frontera; por eso dentro del diamante usa $\lambda=v/f$, no $c/f$.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 2 (PDF pp. 3–4).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 22]].

### 23. Onda de radio dentro de un núcleo de ferrita — **C · prioridad media**

Una onda de radio de frecuencia $f=90\,\mathrm{MHz}$ pasa del vacío a un núcleo aislante de ferrita. A esa frecuencia, sus propiedades relativas son $K=10$ y $K_m=1000$.

**Se pide.** Calcula la longitud de onda en el vacío, la rapidez en la ferrita y la longitud de onda dentro de ella. Indica cuántas veces menor es la longitud de onda en la ferrita que en el vacío.

> [!tip]- Pista de planteo
> Convierte $90\,\mathrm{MHz}$ a $9.0\times10^7\,\mathrm{Hz}$. Luego calcula $\lambda_0=c/f$, $v=c/\sqrt{KK_m}$ y $\lambda_{\mathrm f}=v/f$. La permeabilidad relativa grande también afecta la rapidez.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 3 (PDF p. 4).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 23]].

### 24. Energía y flujo de un frente de onda plano — **C · prioridad media**

En el vacío avanza hacia $+x$ un pulso electromagnético plano. Detrás de un frente ideal, los campos son uniformes y perpendiculares entre sí, con $\vec E\times\vec B$ en $+x$; en un punto de esa región, la magnitud del campo eléctrico es $E=100\,\mathrm{V/m}$. Usa $c=3.00\times10^8\,\mathrm{m/s}$, $\epsilon_0=8.85\times10^{-12}\,\mathrm{F/m}$ y $\mu_0=4\pi\times10^{-7}\,\mathrm{H/m}$.

**Se pide.**

1. Halla la magnitud de $B$.
2. Calcula la densidad total de energía electromagnética $u=u_E+u_B$.
3. Calcula la magnitud del flujo de energía por unidad de área $S$ y comprueba el resultado con $S=cu$.
4. Explica por qué aquí no se promedia un seno ni aparece un factor $1/2$ de promedio temporal.

> [!tip]- Pista de planteo
> Para una onda plana en el vacío, $E=cB$, $u=\frac12\epsilon_0E^2+\frac{B^2}{2\mu_0}$ y $S=EB/\mu_0$. El pulso descrito tiene valores constantes detrás del frente; no es una onda sinusoidal cuyo valor instantáneo oscile.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 4 (PDF pp. 4–5).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 24]].

### 25. Señal de una estación de radio en un satélite — **C · prioridad media**

Una estación transmite una potencia media total $P=50\,\mathrm{kW}$ sobre terreno plano. Supón que no hay pérdidas y que la potencia se reparte uniformemente por todas las direcciones del hemisferio superior. Un satélite está a $r=100\,\mathrm{km}$ de la antena, medidos desde ella. Usa $c=3.00\times10^8\,\mathrm{m/s}$ y $\epsilon_0=8.85\times10^{-12}\,\mathrm{F/m}$.

**Se pide.** Calcula en la posición del satélite:

1. El área hemisférica atravesada por la onda y la intensidad media $I$.
2. La amplitud máxima $E_{max}$ del campo eléctrico.
3. La amplitud máxima $B_{max}$ del campo magnético.

![[imagenes/radiacion-hemisferica-antena.svg]]

> [!tip]- Pista de planteo
> La potencia cruza un hemisferio, cuya área es $2\pi r^2$. Después usa $I=P/(2\pi r^2)$ y, para una onda sinusoidal, $I=\frac12\epsilon_0cE_{max}^2$ y $B_{max}=E_{max}/c$.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 5 (PDF pp. 5–7).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 25]].

### 26. Presión de radiación sobre paneles solares — **C · ampliación**

Un satélite tiene paneles solares de área total $A=4.0\,\mathrm{m^2}$. La radiación solar llega perpendicularmente a los paneles y se absorbe por completo. En la órbita del satélite, la intensidad media es $I=1.4\times10^3\,\mathrm{W/m^2}$. Usa $c=3.00\times10^8\,\mathrm{m/s}$.

**Se pide.** Calcula la potencia media absorbida, la presión de radiación y la fuerza media ejercida sobre los paneles. Indica la dirección de esa fuerza.

> [!tip]- Pista de planteo
> La potencia recibida es $P=IA$. Para una superficie que absorbe la radiación a incidencia normal, $p_{rad}=I/c$ y $F=p_{rad}A$. La fuerza apunta en el sentido de propagación de la luz.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 6 (PDF p. 7).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 26]].

### 27. Flujo medio en una onda estacionaria — **C · ampliación**

Dos ondas planas sinusoidales de igual frecuencia, igual amplitud eléctrica $E_0$ y la misma polarización se propagan en sentidos opuestos por el vacío. En la dirección $x$, los campos de cada onda son

$$
\begin{aligned}
\vec E_+(x,t)&=\hat y E_0\cos(kx-\omega t),&
\vec B_+(x,t)&=\hat z\frac{E_0}{c}\cos(kx-\omega t),\\
\vec E_-(x,t)&=\hat y E_0\cos(kx+\omega t),&
\vec B_-(x,t)&=-\hat z\frac{E_0}{c}\cos(kx+\omega t).
\end{aligned}
$$

**Se pide.** Suma los campos para obtener $\vec E$ y $\vec B$ totales; calcula la componente $x$ del vector de Poynting $\vec S=(\vec E\times\vec B)/\mu_0$ y promedia sobre un período. Explica qué significa el promedio para el transporte neto de energía.

> [!tip]- Pista de planteo
> Usa las identidades $\cos(a-b)+\cos(a+b)=2\cos a\cos b$ y $\cos(a-b)-\cos(a+b)=2\sin a\sin b$. El promedio temporal de $\sin(2\omega t)$ sobre un período es cero.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 7 (PDF p. 8).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 27]].

### 28. Modo electromagnético fundamental en una cavidad — **C · prioridad media**

Dos paredes planas, paralelas y altamente conductoras están separadas por $L=1.50\,\mathrm{cm}$. Entre ellas se establece en el vacío una onda electromagnética estacionaria con el campo eléctrico paralelo a las paredes.

![[imagenes/cavidad-modo-fundamental.svg]]

**Se pide.**

1. Calcula la longitud de onda más larga permitida y la frecuencia más baja distinta de cero.
2. Para ese modo, indica dónde se anula el campo eléctrico y dónde alcanza su amplitud máxima.
3. Indica dónde se anula el campo magnético y dónde alcanza su amplitud máxima.
4. Justifica por qué el patrón debe acomodar media longitud de onda entre las paredes.

> [!tip]- Pista de planteo
> En una pared conductora ideal, la componente tangencial de $\vec E$ debe anularse. Para el modo fundamental, las paredes son dos nodos consecutivos de $E$, separados por $L=\lambda/2$. Luego usa $f=c/\lambda$; los nodos y antinodos de $B$ quedan intercambiados con los de $E$.

**Familia de origen:** material de problemas de ondas electromagnéticas, problema 8 (PDF pp. 8–9).

**Para comparar después:** [[Resoluciones/04 - Ondas electromagnéticas|resolución 28]].

## Clave breve

> [!example]- Abrir solo después de intentar
>
> **20.** $f=8.57\times10^{14}\,\mathrm{Hz}$; $E_{max}=6.45\times10^5\,\mathrm{V/m}$; $k=1.795\times10^7\,\mathrm{rad/m}$; $\omega=5.39\times10^{15}\,\mathrm{rad/s}$; $\vec B$ apunta en $+\hat z$.
>
> **21.** $f=2.83\times10^{13}\,\mathrm{Hz}$; $B_{max}=5.10\times10^{-3}\,\mathrm T$; $k=5.93\times10^5\,\mathrm{rad/m}$; $\omega=1.78\times10^{14}\,\mathrm{rad/s}$; $\vec B$ apunta en $+\hat y$ y la fase es $kx+\omega t$.
>
> **22.** $\lambda_0=5.89\times10^{-7}\,\mathrm m$; $v_d=1.24\times10^8\,\mathrm{m/s}$; $\lambda_d=2.44\times10^{-7}\,\mathrm m$. La frecuencia se conserva; bajan la rapidez y la longitud de onda.
>
> **23.** $\lambda_0=3.33\,\mathrm m$; $v_f=3.00\times10^6\,\mathrm{m/s}$; $\lambda_f=3.33\times10^{-2}\,\mathrm m=3.33\,\mathrm{cm}$; la longitud de onda se reduce por un factor $100$.
>
> **24.** $B=3.33\times10^{-7}\,\mathrm T$; $u=8.85\times10^{-8}\,\mathrm{J/m^3}$; $S=26.5\,\mathrm{W/m^2}$, dirigido hacia $+x$.
>
> **25.** $I=7.96\times10^{-7}\,\mathrm{W/m^2}$; $E_{max}=2.45\times10^{-2}\,\mathrm{V/m}$; $B_{max}=8.16\times10^{-11}\,\mathrm T$.
>
> **26.** $P=5.6\times10^3\,\mathrm W$; $p_{rad}=4.67\times10^{-6}\,\mathrm{Pa}$; $F=1.87\times10^{-5}\,\mathrm N$, en el sentido de propagación.
>
> **27.** $\vec E=2\hat yE_0\cos(kx)\cos(\omega t)$; $\vec B=2\hat z(E_0/c)\sin(kx)\sin(\omega t)$; $S_x=(E_0^2/\mu_0c)\sin(2kx)\sin(2\omega t)$ y $\langle S_x\rangle=0$.
>
> **28.** $\lambda_1=3.00\,\mathrm{cm}$; $f_1=1.00\times10^{10}\,\mathrm{Hz}=10.0\,\mathrm{GHz}$. $E$ es nulo en las paredes y máximo a mitad de camino; $B$ es máximo junto a las paredes y nulo a mitad de camino.

Las resoluciones desarrolladas están en [[Resoluciones/04 - Ondas electromagnéticas|la guía paso a paso]].

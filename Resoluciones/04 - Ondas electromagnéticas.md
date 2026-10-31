---
tags: [fisica-aplicada, resoluciones, ondas-em]
---

# Resoluciones paso a paso — ondas electromagnéticas

Lee cada resolución con papel y lápiz: antes de cada cálculo, predice qué relación corresponde y por qué. Practica primero en [[Ejercicios/04 - Ondas electromagnéticas]] y consulta [[Teoría/04 - Conceptos de ondas electromagnéticas|los conceptos]] o [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|el formulario]] cuando lo necesites.

---

## 20. De los datos de la onda a las ecuaciones vectoriales

### 1. Interpretación y dibujo

La onda está en el vacío; por tanto, su rapidez es $c$. Se dan $\lambda$ y $B_{max}$, y buscamos la frecuencia y la amplitud eléctrica antes de construir las dos funciones de campo. Para hacer única la respuesta vectorial, usamos la convención declarada en el ejercicio: propagación en $+\hat x$ y campo eléctrico en $+\hat y$.

![[imagenes/onda-electromagnetica.svg]]

### 2. Datos en unidades SI

$$
\lambda=350\,\mathrm{nm}
=350\times10^{-9}\,\mathrm m
=3.50\times10^{-7}\,\mathrm m,
\qquad
B_{max}=2.15\,\mathrm{mT}
=2.15\times10^{-3}\,\mathrm T.
$$

### 3. Frecuencia: conectar el período espacial con la rapidez

En el vacío, la onda recorre una longitud de onda por ciclo, de modo que $c=\lambda f$. Despejamos la magnitud pedida:

$$
f=\frac{c}{\lambda}
=\frac{3.00\times10^8\,\mathrm{m/s}}
{3.50\times10^{-7}\,\mathrm m}
=8.57\times10^{14}\,\mathrm{Hz}.
$$

### 4. Amplitud del campo eléctrico

Para una onda plana en el vacío, Maxwell relaciona las amplitudes mediante $E_{max}=cB_{max}$. La usamos porque conocemos $B_{max}$ y buscamos $E_{max}$:

$$
E_{max}
=(3.00\times10^8\,\mathrm{m/s})
(2.15\times10^{-3}\,\mathrm T)
=6.45\times10^5\,\mathrm{V/m}.
$$

La unidad también cuadra: $\mathrm{m/s}\cdot\mathrm T=\mathrm{V/m}$.

### 5. Número de onda y frecuencia angular

El número de onda mide cuánto cambia la fase por metro y $\omega$ cuánto cambia por segundo:

$$
k=\frac{2\pi}{\lambda}
=\frac{2\pi}{3.50\times10^{-7}\,\mathrm m}
=1.795\times10^7\,\mathrm{rad/m},
$$

$$
\omega=2\pi f
=2\pi(8.57\times10^{14}\,\mathrm{Hz})
=5.39\times10^{15}\,\mathrm{rad/s}.
$$

Control equivalente: $ck\approx\omega$.

### 6. Dirección del campo magnético

La propagación tiene vector unitario $\hat n=+\hat x$ y $\vec E_{max}$ apunta en $+\hat y$. Como $\hat x\times\hat y=\hat z$,

$$
\vec B_{max}=+\hat z B_{max}.
$$

Se verifica además $\vec E_{max}\times\vec B_{max}=(+\hat y)\times(+\hat z)=+\hat x$, que coincide con el avance.

### 7. Ecuaciones vectoriales

La onda viaja en $+x$, así que la fase es $kx-\omega t$. Los dos campos están en fase:

$$
\vec E(x,t)
=+\hat y(6.45\times10^5\,\mathrm{V/m})
\cos\left[(1.795\times10^7\,\mathrm{rad/m})x
-(5.39\times10^{15}\,\mathrm{rad/s})t\right],
$$

$$
\vec B(x,t)
=+\hat z(2.15\times10^{-3}\,\mathrm T)
\cos\left[(1.795\times10^7\,\mathrm{rad/m})x
-(5.39\times10^{15}\,\mathrm{rad/s})t\right].
$$

### 8. Control final

- $E_{max}/B_{max}=6.45\times10^5/(2.15\times10^{-3})=3.00\times10^8\,\mathrm{m/s}=c$.
- La fase $kx-\omega t$ avanza en $+x$.
- $(+\hat y)\times(+\hat z)=+\hat x$.

**Resultado:** $f=8.57\times10^{14}\,\mathrm{Hz}$, $E_{max}=6.45\times10^5\,\mathrm{V/m}$ y los campos quedan descritos por las funciones anteriores.

---

## 21. Onda láser que avanza hacia $-x$

### 1. Interpretación y datos

La onda sinusoidal se propaga en el vacío hacia $-\hat x$. La amplitud eléctrica está en $+\hat z$ por la convención del ejercicio. Convertimos primero:

$$
\lambda=10.6\,\mathrm{\mu m}
=10.6\times10^{-6}\,\mathrm m
=1.06\times10^{-5}\,\mathrm m,
\qquad
E_{max}=1.53\,\mathrm{MV/m}
=1.53\times10^6\,\mathrm{V/m}.
$$

### 2. Frecuencia

Usamos $c=\lambda f$ porque se conoce la longitud de onda en el vacío:

$$
f=\frac{c}{\lambda}
=\frac{3.00\times10^8\,\mathrm{m/s}}
{1.06\times10^{-5}\,\mathrm m}
=2.830\times10^{13}\,\mathrm{Hz}.
$$

### 3. Amplitud magnética

De $E_{max}=cB_{max}$ despejamos $B_{max}$:

$$
B_{max}=\frac{E_{max}}{c}
=\frac{1.53\times10^6\,\mathrm{V/m}}
{3.00\times10^8\,\mathrm{m/s}}
=5.10\times10^{-3}\,\mathrm T.
$$

### 4. Número de onda y frecuencia angular

$$
k=\frac{2\pi}{\lambda}
=\frac{2\pi}{1.06\times10^{-5}\,\mathrm m}
=5.927\times10^5\,\mathrm{rad/m},
$$

$$
\omega=2\pi f
=2\pi(2.830\times10^{13}\,\mathrm{Hz})
=1.778\times10^{14}\,\mathrm{rad/s}.
$$

También resulta $\omega=ck$, como debe ocurrir en el vacío.

### 5. Dirección de $\vec B$: aplicar la regla de la mano derecha

La dirección de propagación es $-\hat x$ y $\vec E_{max}$ apunta en $+\hat z$. Entonces

$$
\hat n\times\vec E_{max}
=(-\hat x)\times(+\hat z)
=+\hat y.
$$

Por lo tanto, $\vec B_{max}$ apunta en $+\hat y$. La comprobación equivalente es

$$
(+\hat z)\times(+\hat y)=-\hat x,
$$

que coincide con el sentido de avance.

### 6. Elegir la fase y escribir los campos

Para viajar hacia $-x$ la fase debe ser $kx+\omega t$. Con la convención de amplitudes positivas y los unitarios elegidos:

$$
\vec E(x,t)
=+\hat z(1.53\times10^6\,\mathrm{V/m})
\cos\left[(5.927\times10^5\,\mathrm{rad/m})x
+(1.778\times10^{14}\,\mathrm{rad/s})t\right],
$$

$$
\vec B(x,t)
=+\hat y(5.10\times10^{-3}\,\mathrm T)
\cos\left[(5.927\times10^5\,\mathrm{rad/m})x
+(1.778\times10^{14}\,\mathrm{rad/s})t\right].
$$

### 7. Control y cotejo de signos

Mantener la fase constante da $kx+\omega t=\text{constante}$, por lo que $dx/dt=-\omega/k<0$: la onda sí avanza hacia $-x$. Además, $E_{max}/B_{max}=3.00\times10^8\,\mathrm{m/s}$.

La resolución guardada en Zotero transcribe $\vec E$ en $+\hat z$ y $\vec B$ en $-\hat y$ con esta misma fase. Esos sentidos no son compatibles: $(+\hat z)\times(-\hat y)=+\hat x$, que contradice la propagación en $-\hat x$. Con la orientación $+\hat z$ elegida aquí, el campo magnético compatible es $+\hat y$. Se conserva la condición del enunciado y se corrige el signo para que ambas ecuaciones satisfagan la dirección física de la onda.

**Resultado:** $f=2.83\times10^{13}\,\mathrm{Hz}$, $B_{max}=5.10\times10^{-3}\,\mathrm T$, $k=5.93\times10^5\,\mathrm{rad/m}$ y $\omega=1.78\times10^{14}\,\mathrm{rad/s}$, con los campos y sentidos indicados.

---

## 22. Luz de sodio que atraviesa un diamante

### 1. Qué cambia al cruzar la frontera

La lámpara fija la frecuencia de la luz. Al pasar al diamante, la respuesta eléctrica del material reduce su rapidez. Como $v=\lambda f$ y $f$ se conserva en una frontera estacionaria, la longitud de onda también debe reducirse.

Datos: $f=5.09\times10^{14}\,\mathrm{Hz}$, $K=5.84$, $K_m=1.00$ y $c=3.00\times10^8\,\mathrm{m/s}$.

### 2. Longitud de onda en aire/vacío

Tomamos el índice del aire como uno, de modo que la rapidez es aproximadamente $c$:

$$
\lambda_0=\frac{c}{f}
=\frac{3.00\times10^8\,\mathrm{m/s}}
{5.09\times10^{14}\,\mathrm{s^{-1}}}
=5.89\times10^{-7}\,\mathrm m
=589\,\mathrm{nm}.
$$

### 3. Rapidez y longitud de onda en el diamante

Las constantes relativas del medio reducen la rapidez según $v=c/\sqrt{KK_m}$:

$$
v_d=\frac{3.00\times10^8}{\sqrt{(5.84)(1.00)}}
=1.24\times10^8\,\mathrm{m/s}.
$$

La frecuencia no cambia, así que ahora usamos la rapidez del diamante en $\lambda=v/f$:

$$
\lambda_d=\frac{1.24\times10^8\,\mathrm{m/s}}
{5.09\times10^{14}\,\mathrm{Hz}}
=2.44\times10^{-7}\,\mathrm m
=244\,\mathrm{nm}.
$$

El índice $n=c/v=\sqrt{KK_m}\approx2.42$ permite el control $\lambda_d=\lambda_0/n\approx589/2.42=244\,\mathrm{nm}$. **Cambian la rapidez y la longitud de onda; se conserva la frecuencia.**

---

## 23. Onda de radio dentro de un núcleo de ferrita

### 1. Convertir y elegir el modelo del medio

La frecuencia es $90\,\mathrm{MHz}=9.0\times10^7\,\mathrm{Hz}$. En la ferrita, $K=10$ y $K_m=1000$, por lo que $\sqrt{KK_m}=\sqrt{10000}=100$. La permeabilidad relativa alta es parte del dato y no debe reemplazarse por uno.

### 2. Valores en el vacío

$$
\lambda_0=\frac{c}{f}
=\frac{3.00\times10^8\,\mathrm{m/s}}
{9.0\times10^7\,\mathrm{Hz}}
=3.33\,\mathrm m.
$$

### 3. Valores en la ferrita

$$
v_f=\frac{c}{\sqrt{KK_m}}
=\frac{3.00\times10^8}{100}
=3.00\times10^6\,\mathrm{m/s}.
$$

Como la frecuencia se conserva a través de la frontera,

$$
\lambda_f=\frac{v_f}{f}
=\frac{3.00\times10^6\,\mathrm{m/s}}
{9.0\times10^7\,\mathrm{Hz}}
=3.33\times10^{-2}\,\mathrm m
=3.33\,\mathrm{cm}.
$$

La razón $\lambda_0/\lambda_f=3.33/0.0333=100$ coincide con el índice $n=\sqrt{KK_m}=100$. La longitud de onda se hace cien veces menor dentro de la ferrita.

---

## 24. Energía y flujo de un frente de onda plano

### 1. Relación entre los campos

El frente se mueve en el vacío y los campos son perpendiculares. Para una onda plana $E=cB$, así que

$$
B=\frac{E}{c}
=\frac{100\,\mathrm{V/m}}{3.00\times10^8\,\mathrm{m/s}}
=3.33\times10^{-7}\,\mathrm T.
$$

### 2. Sumar las energías eléctrica y magnética

La densidad total se obtiene sumando las dos formas de energía de campo:

$$
u_E=\frac12\epsilon_0E^2
=\frac12(8.85\times10^{-12})(100)^2
=4.43\times10^{-8}\,\mathrm{J/m^3}.
$$

$$
u_B=\frac{B^2}{2\mu_0}
=\frac{(3.33\times10^{-7})^2}{2(4\pi\times10^{-7})}
=4.42\times10^{-8}\,\mathrm{J/m^3}.
$$

Como se espera para una onda plana en el vacío, ambas contribuciones son iguales dentro del redondeo. Por lo tanto,

$$
u=u_E+u_B=8.85\times10^{-8}\,\mathrm{J/m^3}.
$$

### 3. Flujo de energía

Para una onda que avanza en $+x$, $\vec E\times\vec B$ también debe apuntar en $+x$. La magnitud del vector de Poynting es

$$
S=\frac{EB}{\mu_0}
=\frac{(100)(3.33\times10^{-7})}{4\pi\times10^{-7}}
=26.5\,\mathrm{W/m^2}.
$$

Un control independiente usa $S=cu$:

$$
cu=(3.00\times10^8)(8.85\times10^{-8})
=26.6\,\mathrm{W/m^2},
$$

que coincide al redondear.

### 4. Por qué no se agrega un $1/2$ de promedio

El problema describe un pulso plano con campos constantes detrás de su frente: el valor indicado no es la amplitud de una sinusoide. Se calcula el flujo instantáneo con esos valores. El factor $1/2$ aparece al promediar $\cos^2$ durante un ciclo de una onda sinusoidal; aquí no hay tal ciclo que promediar.

---

## 25. Señal de una estación de radio en un satélite

### 1. Geometría del reparto de potencia

El terreno bloquea la mitad inferior, así que la potencia no se distribuye sobre una esfera completa. El satélite intercepta la onda a $r=100\,\mathrm{km}=1.00\times10^5\,\mathrm m$; el área hemisférica a esa distancia es

![[imagenes/radiacion-hemisferica-antena.svg]]

$$
A=2\pi r^2
=2\pi(1.00\times10^5\,\mathrm m)^2
=6.28\times10^{10}\,\mathrm{m^2}.
$$

### 2. Intensidad a esa distancia

La potencia media $P=50\,\mathrm{kW}=5.00\times10^4\,\mathrm W$ se reparte uniformemente sobre esa área:

$$
I=\frac{P}{A}
=\frac{5.00\times10^4\,\mathrm W}
{6.28\times10^{10}\,\mathrm{m^2}}
=7.96\times10^{-7}\,\mathrm{W/m^2}.
$$

### 3. Amplitud eléctrica y magnética

La señal es sinusoidal, así que la intensidad media se relaciona con la amplitud máxima mediante $I=\frac12\epsilon_0cE_{max}^2$. Despejamos la incógnita antes de sustituir:

$$
E_{max}=\sqrt{\frac{2I}{\epsilon_0c}}
=\sqrt{\frac{2(7.96\times10^{-7})}
{(8.85\times10^{-12})(3.00\times10^8)}}
=2.448\times10^{-2}\,\mathrm{V/m}\approx2.45\times10^{-2}\,\mathrm{V/m}.
$$

Después aplicamos la relación de amplitudes en el vacío:

$$
B_{max}=\frac{E_{max}}{c}
=\frac{2.448\times10^{-2}\,\mathrm{V/m}}
{3.00\times10^8\,\mathrm{m/s}}
=8.16\times10^{-11}\,\mathrm T.
$$

El resultado es pequeño porque la potencia de la antena ya se distribuyó sobre un área de más de $6\times10^{10}\,\mathrm{m^2}$.

---

## 26. Presión de radiación sobre paneles solares

### 1. Potencia media absorbida

La luz incide perpendicularmente y atraviesa un área $A=4.0\,\mathrm{m^2}$. Por definición, $I=P/A$, de donde

$$
P=IA
=(1.4\times10^3\,\mathrm{W/m^2})(4.0\,\mathrm{m^2})
=5.6\times10^3\,\mathrm W.
$$

El satélite absorbe en promedio $5.6\,\mathrm{kW}$.

### 2. Presión y fuerza

Al absorber la radiación, cada unidad de área recibe por segundo el momento correspondiente a la energía incidente. Para absorción completa a incidencia normal, $p_{rad}=I/c$:

$$
p_{rad}=\frac{1.4\times10^3\,\mathrm{W/m^2}}
{3.00\times10^8\,\mathrm{m/s}}
=4.67\times10^{-6}\,\mathrm{Pa}.
$$

La fuerza total es presión por área:

$$
F=p_{rad}A
=(4.67\times10^{-6}\,\mathrm{N/m^2})(4.0\,\mathrm{m^2})
=1.87\times10^{-5}\,\mathrm N.
$$

También se obtiene $F=P/c$, porque $p_{rad}A=IA/c= P/c$. La fuerza apunta en la dirección de propagación de la luz. Si los paneles reflejaran perfectamente la luz, la presión se duplicaría; no es el caso aquí porque se especifica absorción completa.

---

## 27. Flujo medio en una onda estacionaria

### 1. Sumar por separado los campos

Sumamos los campos eléctricos de las dos ondas y aplicamos la identidad de suma de cosenos:

$$
\vec E=\vec E_++\vec E_-
=\hat y E_0[\cos(kx-\omega t)+\cos(kx+\omega t)]
=2\hat y E_0\cos(kx)\cos(\omega t).
$$

Para los campos magnéticos, la onda que retrocede tiene sentido magnético opuesto. Por eso se restan los cosenos:

$$
\vec B=\vec B_++\vec B_-
=\hat z\frac{E_0}{c}[\cos(kx-\omega t)-\cos(kx+\omega t)]
=2\hat z\frac{E_0}{c}\sin(kx)\sin(\omega t).
$$

### 2. Calcular el flujo dirigido

Como $\hat y\times\hat z=\hat x$, el flujo apunta en el eje de propagación de las ondas y su componente es

$$
S_x=\frac{E_yB_z}{\mu_0}
=\frac{E_0^2}{\mu_0c}\sin(2kx)\sin(2\omega t).
$$

El signo cambia con el tiempo: en ciertos instantes la energía fluye hacia $+x$ y en otros hacia $-x$.

### 3. Promediar sobre un período

En un ciclo completo, $\sin(2\omega t)$ tiene promedio cero. Los factores que dependen de $x$ no cambian durante el promedio temporal, así que

$$
\langle S_x\rangle_t
=\frac{E_0^2}{\mu_0c}\sin(2kx)\langle\sin(2\omega t)\rangle_t
=0.
$$

**Interpretación:** los campos existen y la energía fluye instantáneamente, pero no hay transporte neto sostenido hacia un lado en una onda estacionaria ideal. Al hablar de intensidad en este caso, el promedio relevante para el transporte neto es el de la componente dirigida de $\vec S$, no el promedio del valor absoluto.

> [!note] Precisión sobre la redacción del TP
> El enunciado del TP llama intensidad al promedio de la magnitud de $\vec S$, pero la resolución calcula el promedio temporal de la componente firmada $S_x$. Para decidir si existe transporte neto hacia un lado, ese promedio firmado es el apropiado: resulta cero. El promedio de $|\vec S|$ mediría el flujo instantáneo medio sin distinguir sus sentidos y no respondería si hay transporte neto.

---

## 28. Modo electromagnético fundamental en una cavidad

### 1. Condición en las paredes y longitud de onda

En una pared conductora ideal la componente tangencial del campo eléctrico es nula. Las dos paredes, separadas por $L$, deben coincidir con nodos consecutivos de $E$. La distancia entre nodos consecutivos es media longitud de onda; por eso, en el modo fundamental,

$$
L=\frac{\lambda_1}{2},
\qquad
\lambda_1=2L=2(1.50\,\mathrm{cm})=3.00\,\mathrm{cm}
=3.00\times10^{-2}\,\mathrm m.
$$

Este es el modo permitido de mayor longitud de onda. Una longitud mayor no cabría entre los dos nodos de las paredes.

### 2. Frecuencia más baja

La onda se propaga en el vacío entre las paredes, de modo que $c=\lambda f$:

$$
f_1=\frac{c}{\lambda_1}
=\frac{3.00\times10^8\,\mathrm{m/s}}
{3.00\times10^{-2}\,\mathrm m}
=1.00\times10^{10}\,\mathrm{Hz}
=10.0\,\mathrm{GHz}.
$$

### 3. Posición de nodos y máximos

![[imagenes/cavidad-modo-fundamental.svg]]

Para el modo fundamental, la amplitud espacial de $E$ puede representarse como $|E|_{amp}\propto\sin(\pi x/L)$: vale cero en $x=0$ y $x=L$, y es máxima en $x=L/2$. El patrón de amplitud de $B$ es complementario, $|B|_{amp}\propto|\cos(\pi x/L)|$: tiene máximos junto a las paredes y un nodo en el centro.

**Respuesta:** $E=0$ en ambas paredes y alcanza su máximo a $0.75\,\mathrm{cm}$ de cada una. $B$ es máximo junto a las paredes y se anula a mitad de la cavidad. Las amplitudes espaciales describen dónde oscila cada campo con mayor o menor valor; en un nodo el campo permanece nulo para todo instante.

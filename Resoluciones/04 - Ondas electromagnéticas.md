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
---
tags: [fisica-aplicada, ejercicios, ondas-acustica]
---

# Ejercicios — Ondas y acústica

**Conceptos:** [[Teoría/03 - Conceptos de ondas y acústica]] · **Fórmulas:** [[Teoría/03 - Fórmulas aplicadas de ondas y acústica]] · **Resoluciones:** [[Resoluciones/03 - Ondas y acústica]] · **Método:** [[Ejercicios/00 - Método y registro]]

> [!info] Cómo usar esta hoja
> Los ejercicios **M** practican familias presentes en los modelos; **R** son variantes para comprobar que entiendes el principio. Para cada problema escribe datos e incógnita, dibuja la propagación, nombra el modelo, despeja antes de sustituir y comprueba unidad y sentido físico. Abre la pista solo después de intentar.

## 14. Desplazamiento de partículas a partir de presión — **M**

**Situación.** Una onda sonora sinusoidal longitudinal se propaga en el aire. La presión oscila alrededor de la presión atmosférica mientras las partículas del aire se desplazan alrededor de su posición de equilibrio.

**Datos**

- Amplitud máxima de presión: $\Delta p_{\max}=3.0\times10^{-2}\,\mathrm{Pa}$.
- Frecuencia: $f=1000\,\mathrm{Hz}$.
- Rapidez del sonido: $v=344\,\mathrm{m/s}$.
- Módulo volumétrico del aire: $B=1.42\times10^5\,\mathrm{Pa}$.

**Se pide.** Calcula el número de onda $k$ y la amplitud de desplazamiento $s_{\max}$ de las partículas.

![[imagenes/sonido-longitudinal.svg]]

> [!tip]- Pista de planteo
> Usa $k=2\pi f/v$. La deformación compresional de una onda sinusoidal conecta las dos amplitudes con $\Delta p_{\max}=Bks_{\max}$. Despeja $s_{\max}$.

**Familia de origen:** práctica Sonido, ejercicio 1; tipo también incluido en el modelo 2025.

## 15. Intensidad y nivel sonoro — **R**

**Situación.** Un micrófono mide una onda sonora sinusoidal progresiva en aire. El dato de presión es la amplitud máxima, no el valor eficaz.

**Datos**

- $\Delta p_{\max}=0.020\,\mathrm{Pa}$.
- Densidad del aire: $\rho=1.20\,\mathrm{kg/m^3}$.
- Rapidez del sonido: $v=343\,\mathrm{m/s}$.
- Intensidad de referencia: $I_0=1.0\times10^{-12}\,\mathrm{W/m^2}$.

**Se pide.** Calcula la intensidad media $I$ y el nivel sonoro $\beta$ en dB.

![[imagenes/sonido-longitudinal.svg]]

> [!tip]- Pista de planteo
> Primero calcula $I=(\Delta p_{\max})^2/(2\rho v)$. Después compara esa intensidad con $I_0$ mediante el logaritmo decimal.

**Familia de origen:** práctica Sonido, ejercicios 6 y 9.

## 16. Nivel sonoro con una y dos máquinas — **M**

**Situación.** Dos máquinas idénticas están a la misma distancia de un trabajador. La intensidad indicada para cada máquina funcionando en el puesto del trabajador es la transcripta del modelo escaneado.

**Datos**

- Intensidad de una máquina: $I=2.0\times10^7\,\mathrm{W/m^2}$.
- Intensidad de referencia: $I_0=1.0\times10^{-12}\,\mathrm{W/m^2}$.
- Las máquinas son independientes: sus intensidades se suman.

**Se pide.**

1. Calcula el nivel sonoro con una máquina funcionando.
2. Calcula el nivel con las dos máquinas funcionando.
3. Explica cuánto aumenta el nivel al duplicar la intensidad.

> [!warning] Dato leído en el modelo
> El escaneo imprime $2.0\times10^7\,\mathrm{W/m^2}$. Es un valor extraordinariamente alto para sonido, pero el exponente se verificó visualmente; en este ejercicio se conserva el dato literal.

> [!tip]- Pista de planteo
> Calcula $\beta_1=10\log_{10}(I/I_0)$. Para dos fuentes, suma primero $I_{\mathrm{tot}}=2I$ y aplica el logaritmo una segunda vez.

**Familia de origen:** modelo 2023, pregunta 2.

## 17. Doppler: fuente que se acerca — **M**

**Situación.** Una ambulancia se acerca a un observador quieto respecto del aire. La fuente emite frentes sucesivos desde posiciones cada vez más cercanas al observador.

**Datos**

- Frecuencia emitida: $f_s=500\,\mathrm{Hz}$.
- Rapidez del sonido en aire: $v=340\,\mathrm{m/s}$.
- Rapidez de la ambulancia hacia el observador: $v_s=50\,\mathrm{m/s}$.
- Observador quieto: $v_o=0$.

**Se pide.** Calcula la frecuencia recibida $f_{\mathrm{obs}}$.

![[imagenes/doppler-casos.svg]]

> [!tip]- Pista de planteo
> La fuente que se acerca acorta la longitud de onda por delante. Usa $f_{\mathrm{obs}}=f_s\,v/(v-v_s)$ y comprueba que el resultado sea mayor que $500\,\mathrm{Hz}$.

**Familia de origen:** modelo 2024, pregunta 3a.

## 18. Doppler: observador que se aleja — **M**

**Situación.** La sirena permanece en reposo respecto del aire. El observador se aleja de ella; por eso encuentra menos frentes de onda por segundo.

**Datos**

- Frecuencia emitida: $f_s=500\,\mathrm{Hz}$.
- Rapidez del sonido: $v=340\,\mathrm{m/s}$.
- Rapidez del observador alejándose: $30\,\mathrm{m/s}$.
- Fuente quieta respecto del medio: $v_s=0$.

**Se pide.** Calcula $f_{\mathrm{obs}}$.

![[imagenes/doppler-casos.svg]]

> [!tip]- Pista de planteo
> Con esta convención, alejarse significa $v_o=-30\,\mathrm{m/s}$. La fuente quieta deja $\lambda=v/f_s$; el observador se encuentra con los frentes a rapidez $v-30\,\mathrm{m/s}$.

**Familia de origen:** modelo 2024, pregunta 3b.

## 19. Doppler: fuente y observador se acercan — **R**

**Situación.** Una sirena y una persona se desplazan una hacia la otra respecto del aire. El medio permanece en reposo.

**Datos**

- Frecuencia emitida: $f_s=500\,\mathrm{Hz}$.
- Rapidez del sonido: $v=340\,\mathrm{m/s}$.
- La fuente se mueve hacia el observador a $v_s=40\,\mathrm{m/s}$.
- El observador se mueve hacia la fuente a $v_o=20\,\mathrm{m/s}$.

**Se pide.** Calcula la frecuencia recibida y separa en tu explicación el efecto de la fuente del efecto del observador.

![[imagenes/doppler-casos.svg]]

> [!tip]- Pista de planteo
> Ambos movimientos son de acercamiento: $v_o>0$ y $v_s>0$. La fuente acorta $\lambda$ y el observador aumenta su rapidez de encuentro con los frentes.

**Familia de origen:** variante de transferencia de los casos por separado del modelo 2024.

## Clave breve

> [!example]- Abrir después de resolver
> 14. $k=18.27\,\mathrm{rad/m}$; $s_{\max}=1.16\times10^{-8}\,\mathrm{m}=11.6\,\mathrm{nm}$.
>
> 15. $I=4.86\times10^{-7}\,\mathrm{W/m^2}$; $\beta=56.9\,\mathrm{dB}$.
>
> 16. Una máquina: $193.0\,\mathrm{dB}$; dos: $196.0\,\mathrm{dB}$; aumento: $3.01\,\mathrm{dB}$.
>
> 17. $f_{\mathrm{obs}}=586.2\,\mathrm{Hz}$.
>
> 18. $f_{\mathrm{obs}}=455.9\,\mathrm{Hz}$.
>
> 19. $f_{\mathrm{obs}}=600\,\mathrm{Hz}$.

---
tags: [fisica-aplicada, ejercicios, ondas-acustica]
---

# Ejercicios — Ondas y acústica

**Conceptos:** [[Teoría/03 - Conceptos de ondas y acústica]] · **Fórmulas:** [[Teoría/03 - Fórmulas aplicadas de ondas y acústica]] · **Resoluciones:** [[Resoluciones/03 - Ondas y acústica]] · **Método:** [[Ejercicios/00 - Método y registro]]

> [!info] Cómo usar esta hoja
> Los ejercicios **M** practican familias presentes en los modelos; **R** son variantes de esos formatos; **C** amplían la práctica con temas del TP que no aparecieron en los modelos revisados. Para cada problema escribe datos e incógnita, dibuja la propagación, nombra el modelo, despeja antes de sustituir y comprueba unidad y sentido físico. Abre la pista solo después de intentar.

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

## 20. Rapidez del sonido y longitudes de onda en distintos medios — **C · prioridad media**

El TP incluye problemas donde debes escoger la expresión de rapidez adecuada al material. En cada inciso, usa solo el modelo de ese medio.

### a) Sonido en agua

Una onda de frecuencia $f=262\,\mathrm{Hz}$ se propaga en agua. Usa el módulo volumétrico $B=2.20\times10^9\,\mathrm{Pa}$ y la densidad $\rho=1.00\times10^3\,\mathrm{kg/m^3}$.

**Se pide.** Calcula la rapidez del sonido y la longitud de onda en el agua.

### b) Onda longitudinal en una varilla de plomo

Para una varilla delgada de plomo, toma $Y=1.60\times10^{10}\,\mathrm{Pa}$ y $\rho=1.13\times10^4\,\mathrm{kg/m^3}$.

**Se pide.** Estima la rapidez de propagación de una onda longitudinal en la varilla.

### c) Sonido en aire y rango audible

El aire se modela como gas ideal a $T=20\,^\circ\mathrm C$, con $\gamma=1.40$, masa molar media $M=28.8\times10^{-3}\,\mathrm{kg/mol}$ y $R=8.314\,\mathrm{J/(mol\,K)}$.

**Se pide.**

1. Calcula la rapidez del sonido. Convierte primero la temperatura a kelvin.
2. Calcula las longitudes de onda correspondientes a $20\,\mathrm{Hz}$ y $20\,000\,\mathrm{Hz}$.
3. Indica cuál de las dos es la longitud de onda mayor.

> [!tip]- Pista de planteo
> Agua: $v=\sqrt{B/\rho}$ y después $\lambda=v/f$. Varilla: $v\approx\sqrt{Y/\rho}$. Gas ideal: $v=\sqrt{\gamma RT/M}$; al final usa de nuevo $\lambda=v/f$.

**Familias de origen:** TP de sonido 2021, ejercicios 3–5. Datos de propiedades explicitados para que no dependas de tablas externas.

## 21. Igual intensidad con dos frecuencias — **C · prioridad media**

Dos ondas sinusoidales progresivas se propagan en el mismo aire. La primera tiene $f_1=1000\,\mathrm{Hz}$ y amplitud máxima de presión $\Delta p_{1,\max}=3.0\times10^{-2}\,\mathrm{Pa}$. La segunda tiene $f_2=20\,\mathrm{Hz}$ y se ajusta para tener **la misma intensidad media**.

Usa para ambas $\rho=1.20\,\mathrm{kg/m^3}$ y $v=344\,\mathrm{m/s}$.

**Se pide.**

1. Calcula la intensidad común.
2. Calcula la amplitud máxima de presión de la segunda onda.
3. Calcula la amplitud de desplazamiento de las partículas para ambas frecuencias y compara los resultados.

> [!tip]- Pista de planteo
> En el mismo medio, $I=\Delta p_{\max}^2/(2\rho v)$. Igual intensidad implica igual presión máxima. Para el desplazamiento usa $s_{\max}=\Delta p_{\max}/(\rho v\,2\pi f)$.

**Familia de origen:** TP de sonido 2021, ejercicio 7.

## 22. Transmisión de presión al fluido del oído — **C · prioridad baja**

Una onda sonora en aire tiene amplitud máxima de presión $\Delta p_{\mathrm{aire},\max}=3.0\times10^{-2}\,\mathrm{Pa}$ y frecuencia $f=1000\,\mathrm{Hz}$. En el modelo simplificado del TP, la fuerza transmitida por los huesecillos se conserva mientras el área efectiva cambia:

- área móvil del tímpano: $A_t=43\,\mathrm{mm^2}$;
- área de contacto del estribo: $A_e=3.2\,\mathrm{mm^2}$.

En el fluido del oído interno usa $v_f=1500\,\mathrm{m/s}$ y $\rho_f=1.00\times10^3\,\mathrm{kg/m^3}$.

**Se pide.**

1. Calcula la amplitud de presión transmitida al fluido.
2. Calcula la amplitud de desplazamiento de la onda en ese fluido.

> [!warning] Alcance del modelo
> Se conserva la fuerza y se concentra sobre el área del estribo, como idealiza el ejercicio. La densidad del fluido se aproxima a la del agua para poder calcular el desplazamiento.

> [!tip]- Pista de planteo
> Usa $F=pA$: $p_f A_e=\Delta p_{\mathrm{aire},\max}A_t$. Luego aplica al fluido $s_{\max}=p_{f,\max}/(\rho_fv_f\,2\pi f)$.

**Familia de origen:** TP de sonido 2021, ejercicio 2.

## 23. Potencia acústica y cambio con la distancia — **C · prioridad media**

Un conjunto de altavoces se modela como una fuente puntual que emite isotrópicamente. A $r_1=20\,\mathrm m$ produce una intensidad $I_1=1.0\,\mathrm{W/m^2}$. Usa $I_0=1.0\times10^{-12}\,\mathrm{W/m^2}$.

**Se pide.**

1. Calcula la potencia acústica total de la fuente.
2. Calcula la intensidad a $r_2=40\,\mathrm m$.
3. ¿Cuántos decibeles cambia el nivel entre esas dos distancias?
4. Calcula las intensidades que corresponden a niveles de $28\,\mathrm{dB}$ y $92\,\mathrm{dB}$.

> [!tip]- Pista de planteo
> Primero aplica $P_{\mathrm{ac}}=4\pi r_1^2I_1$. La fuente conserva la potencia y la intensidad se reparte sobre $4\pi r^2$. Para el cambio de nivel basta $\Delta\beta=10\log_{10}(I_2/I_1)$. Para el último inciso despeja $\beta=10\log_{10}(I/I_0)$ como $I=I_0\,10^{\beta/10}$.

**Familias de origen:** TP de sonido 2021, ejercicios 8–10. Se combinan potencia, cambio de nivel con la distancia e inversión de la escala de decibeles.

## 24. Interferencia de dos altavoces coherentes — **C · prioridad baja**

Dos altavoces pequeños reciben la misma señal y emiten en fase. En el punto $P$, las distancias son $r_A=5.00\,\mathrm m$ desde el altavoz A y $r_B=4.00\,\mathrm m$ desde el altavoz B. La rapidez del sonido es $v=350\,\mathrm{m/s}$.

**Se pide.**

1. Calcula la diferencia de caminos.
2. Encuentra las tres frecuencias positivas más bajas que producen interferencia constructiva en $P$.
3. Encuentra las tres frecuencias positivas más bajas que producen interferencia destructiva en $P$.

> [!tip]- Pista de planteo
> Como las fuentes emiten en fase, usa $\Delta r=m\lambda$ para máximos y $\Delta r=(m+\tfrac12)\lambda$ para mínimos. Sustituye $\lambda=v/f$ y ordena las frecuencias positivas.

**Familia de origen:** TP de sonido 2021, ejercicio 12. Las dos longitudes de camino se explicitan para hacer transparente el planteo geométrico.

## 25. Cancelación del sonido reflejado por una pared — **C · prioridad baja**

Un altavoz emite un tono de $f=680\,\mathrm{Hz}$ perpendicularmente hacia una pared rígida. En el aire, la rapidez del sonido es $v=340\,\mathrm{m/s}$. Considera la superposición ideal de la onda incidente y la reflejada.

**Se pide.** Calcula las tres primeras distancias desde la pared donde la variación de presión acústica se anula.

> [!tip]- Pista de planteo
> Calcula $\lambda=v/f$. Para una pared rígida, los primeros nodos de presión se encuentran en $x=(2n+1)\lambda/4$, con $n=0,1,2,\ldots$.

**Familia de origen:** TP de sonido 2021, ejercicio 11.

## 26. Longitud de onda delante y detrás de una sirena; frecuencia del eco — **C · prioridad media**

Una sirena de frecuencia $f_s=300\,\mathrm{Hz}$ se mueve a $v_s=30\,\mathrm{m/s}$ hacia una pared fija. La rapidez del sonido en el aire es $v=340\,\mathrm{m/s}$.

**Se pide.**

1. Calcula la longitud de onda si la sirena estuviera quieta.
2. Calcula las longitudes de onda delante y detrás de la sirena mientras se mueve.
3. Calcula la frecuencia del eco que recibe el conductor al reflejarse el sonido en la pared.

> [!tip]- Pista de planteo
> Delante: $\lambda_{\mathrm{delante}}=(v-v_s)/f_s$. Detrás: $\lambda_{\mathrm{detrás}}=(v+v_s)/f_s$. Para el eco, calcula primero la frecuencia que recibe la pared y después la que recibe la sirena móvil.

**Familias de origen:** TP de sonido 2021, ejercicios 13 y 17.

## 27. Fuente y observador en movimiento simultáneo — **C · prioridad media**

Una sirena emite a $f_s=300\,\mathrm{Hz}$. Respecto del aire, la fuente se aleja del receptor a $45\,\mathrm{m/s}$ mientras el receptor se mueve hacia la sirena a $15\,\mathrm{m/s}$. Usa $v=340\,\mathrm{m/s}$.

**Se pide.** Calcula la frecuencia recibida y explica por qué puede quedar por debajo de $300\,\mathrm{Hz}$ aunque el receptor se acerque.

> [!tip]- Pista de planteo
> Con la convención de esta guía, $v_s=-45\,\mathrm{m/s}$ y $v_o=+15\,\mathrm{m/s}$. Sustituye ambos signos en $f_{\mathrm{obs}}=f_s(v+v_o)/(v-v_s)$.

**Familia de origen:** TP de sonido 2021, ejercicio 16; combina los dos movimientos en un sentido distinto al modelo 2024.

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
>
> 20. Agua: $v=1483\,\mathrm{m/s}$, $\lambda=5.66\,\mathrm m$; plomo: $v=1190\,\mathrm{m/s}$; aire: $v=344\,\mathrm{m/s}$ y rango $\lambda=17.2\,\mathrm m$ a $0.0172\,\mathrm m$.
>
> 21. $I=1.09\times10^{-6}\,\mathrm{W/m^2}$; $\Delta p_{2,\max}=0.030\,\mathrm{Pa}$; $s_{1,\max}=1.16\times10^{-8}\,\mathrm m$, $s_{2,\max}=5.78\times10^{-7}\,\mathrm m$.
>
> 22. $p_{f,\max}=0.403\,\mathrm{Pa}$; $s_{f,\max}=4.28\times10^{-11}\,\mathrm m$.
>
> 23. $P_{\mathrm{ac}}=5.03\times10^3\,\mathrm W$; $I_2=0.250\,\mathrm{W/m^2}$; $\Delta\beta=-6.02\,\mathrm{dB}$; $I(28\,\mathrm{dB})=6.31\times10^{-10}\,\mathrm{W/m^2}$; $I(92\,\mathrm{dB})=1.58\times10^{-3}\,\mathrm{W/m^2}$.
>
> 24. $\Delta r=1.00\,\mathrm m$; constructiva: $350$, $700$, $1050\,\mathrm{Hz}$; destructiva: $175$, $525$, $875\,\mathrm{Hz}$.
>
> 25. $\lambda=0.500\,\mathrm m$; nodos a $0.125$, $0.375$ y $0.625\,\mathrm m$ de la pared.
>
> 26. $\lambda_0=1.133\,\mathrm m$; delante $1.033\,\mathrm m$; detrás $1.233\,\mathrm m$; eco $f_{\mathrm{eco}}=358.1\,\mathrm{Hz}$.
>
> 27. $f_{\mathrm{obs}}=276.6\,\mathrm{Hz}$.

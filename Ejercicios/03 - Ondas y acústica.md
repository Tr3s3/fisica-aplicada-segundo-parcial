---
tags: [fisica-aplicada, ejercicios, ondas-acustica]
---

# Ejercicios — Ondas y acústica

**Teoría:** [[Teoría/03 - Ondas y acústica]] · **Resoluciones:** [[Resoluciones/03 - Ondas y acústica]] · **Método:** [[Ejercicios/00 - Método y registro]]

> [!info] Cómo usar esta hoja
> Se conserva la numeración global para que coincida con el plan. **M** reproduce un tipo de los modelos; **R** es una variante de entrenamiento. Resuelve primero sin abrir la pista; consulta la clave al final.

## Ejercicios del tema

### 14. Desplazamiento de partículas a partir de presión — **M**

**Situación.** En una onda sonora longitudinal, la presión varía mientras las partículas del aire oscilan alrededor de su posición de equilibrio.

**Datos**

- Amplitud de presión: $\Delta p_{max}=3.0\times10^{-2}\,\mathrm{Pa}$.
- Frecuencia: $f=1000\,\mathrm{Hz}$.
- Rapidez del sonido: $v=344\,\mathrm{m/s}$.
- Módulo volumétrico del aire: $B=1.42\times10^5\,\mathrm{Pa}$.

**Se pide.** Calcula la amplitud de desplazamiento $s_{max}$ de las partículas.

![[imagenes/sonido-longitudinal.svg]]

> [!tip]- Pista de arranque
>
> Primero calcula $k=2\pi f/v$. Después usa la relación entre presión y desplazamiento $\Delta p_{max}=Bk s_{max}$. Despeja $s_{max}$ y conserva unidades SI.

**Para comparar después:** [[Resoluciones/03 - Ondas y acústica]].

### 15. Intensidad sonora y nivel en decibeles — **R**

**Situación.** La amplitud de presión permite hallar la intensidad media de una onda sonora progresiva; luego se compara esa intensidad con el umbral de referencia.

**Datos**

- $\Delta p_{max}=0.020\,\mathrm{Pa}$.
- Densidad del aire: $\rho=1.20\,\mathrm{kg/m^3}$.
- Rapidez del sonido: $v=343\,\mathrm{m/s}$.
- Intensidad de referencia: $I_0=1.0\times10^{-12}\,\mathrm{W/m^2}$.

**Se pide.** Calcula la intensidad $I$ y el nivel $\beta$ en dB.

![[imagenes/sonido-longitudinal.svg]]

> [!tip]- Pista de arranque
>
> Para una onda sinusoidal, $I=(\Delta p_{max})^2/(2\rho v)$. Luego usa $\beta=10\log_{10}(I/I_0)$. El logaritmo se aplica a la razón sin unidades.

### 16. Nivel sonoro de una o dos máquinas — **M**

**Situación.** Dos máquinas independientes producen sonido en el mismo puesto de trabajo. El modelo escaneado parece indicar $10^7\,\mathrm{W/m^2}$, aunque conviene revisar el exponente en tu copia.

**Datos**

- Intensidad por máquina: $I=2.0\times10^7\,\mathrm{W/m^2}$ según la lectura del escaneo.
- Intensidad de referencia: $I_0=1.0\times10^{-12}\,\mathrm{W/m^2}$.
- Para dos máquinas iguales e independientes, las intensidades se suman.

**Se pide.** Calcula el nivel con una máquina y con dos. Explica cuánto cambia el nivel al duplicar la intensidad.

> [!tip]- Pista de arranque
>
> Calcula $\beta_1=10\log_{10}(I/I_0)$. Para dos fuentes, usa $I_{tot}=2I$ y vuelve a calcular el nivel; no sumes directamente los decibeles.

### 17. Doppler: fuente que se acerca — **M**

**Situación.** Una sirena se mueve hacia una persona quieta respecto del aire. Los frentes de onda delante de la fuente quedan más próximos.

**Datos**

- Frecuencia emitida: $f=500\,\mathrm{Hz}$.
- Rapidez del sonido: $v_{snd}=340\,\mathrm{m/s}$.
- Rapidez de la fuente hacia el observador: $v_s=50\,\mathrm{m/s}$.
- Observador en reposo: $v_o=0$.

**Se pide.** Calcula la frecuencia recibida $f'$.

![[imagenes/doppler-sonido.svg]]

> [!tip]- Pista de arranque
>
> Para fuente que se acerca y observador quieto, $f'=f\,v_{snd}/(v_{snd}-v_s)$. El denominador disminuye, así que la frecuencia observada debe superar los $500\,\mathrm{Hz}$ emitidos.

**Para comparar después:** [[Resoluciones/03 - Ondas y acústica]].

### 18. Doppler: observador que se aleja — **M**

**Situación.** La sirena permanece quieta y el observador se aleja de ella a través del aire.

**Datos**

- Frecuencia emitida: $f=500\,\mathrm{Hz}$.
- Rapidez del sonido: $v_{snd}=340\,\mathrm{m/s}$.
- Rapidez del observador alejándose: $v_o=30\,\mathrm{m/s}$.
- Fuente en reposo: $v_s=0$.

**Se pide.** Calcula la frecuencia recibida $f'$.

> [!tip]- Pista de arranque
>
> Para una fuente quieta y un observador que se aleja, $f'=f(v_{snd}-v_o)/v_{snd}$. La frecuencia recibida debe ser menor que la emitida.

**Para comparar después:** [[Resoluciones/03 - Ondas y acústica]].

### 19. Doppler: fuente y observador se acercan — **R**

**Situación.** La fuente y el observador se aproximan uno al otro respecto del aire. Distingue el movimiento de quien emite del movimiento de quien recibe.

**Datos**

- Frecuencia emitida: $f=500\,\mathrm{Hz}$.
- Rapidez del sonido: $v_{snd}=340\,\mathrm{m/s}$.
- Fuente hacia el observador: $v_s=40\,\mathrm{m/s}$.
- Observador hacia la fuente: $v_o=20\,\mathrm{m/s}$.

**Se pide.** Calcula la frecuencia recibida.

![[imagenes/doppler-sonido.svg]]

> [!tip]- Pista de arranque
>
> Con ambos acercándose, $f'=f(v_{snd}+v_o)/(v_{snd}-v_s)$. El movimiento del observador modifica el numerador; el de la fuente modifica el denominador.

## Clave breve

> [!example]- Clave breve — abrir solo después de intentar
>
> 14. $k=18.27\,\mathrm{rad/m}$; $s_{max}=1.16\times10^{-8}\,\mathrm{m}$.
> 15. $I=4.86\times10^{-7}\,\mathrm{W/m^2}$; $\beta=56.9\,\mathrm{dB}$.
> 16. Si $I=2.0\times10^7\,\mathrm{W/m^2}$: una máquina $193.0\,\mathrm{dB}$; dos $196.0\,\mathrm{dB}$. Si el original dice $2.0\times10^{-7}$, son $53.0$ y $56.0\,\mathrm{dB}$. Duplicar la intensidad aumenta el nivel en $3.01\,\mathrm{dB}$.
> 17. $f'=586.2\,\mathrm{Hz}$.
> 18. $f'=455.9\,\mathrm{Hz}$.
> 19. $f'=600\,\mathrm{Hz}$.

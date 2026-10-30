---
tags: [fisica-aplicada, ejercicios, gravitacion]
---

# Ejercicios — Gravitación y órbitas

**Teoría:** [[Teoría/01 - Gravitación y órbitas]] · **Resoluciones:** [[Resoluciones/01 - Gravitación y órbitas]] · **Método:** [[Ejercicios/00 - Método y registro]]

> [!info] Cómo usar esta hoja
> Se conserva la numeración global para que coincida con el plan. **M** reproduce un tipo de los modelos; **R** es una variante de entrenamiento. Resuelve primero sin abrir la pista; consulta la clave al final.

## Ejercicios del tema

### 1. Campo gravitatorio de dos masas simétricas — **M**

**Situación.** Dos masas iguales atraen una partícula de prueba situada sobre el eje de simetría. La partícula de prueba no altera el campo que se quiere calcular.

**Datos**

- $M_1=M_2=0.260\,\mathrm{kg}$.
- Separación entre las masas: $16.0\,\mathrm{cm}$.
- $P$ está $6.0\,\mathrm{cm}$ arriba del punto medio y a $10.0\,\mathrm{cm}$ de cada masa.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula el módulo y la dirección de $\vec g(P)$.

![[imagenes/campo-gravitatorio.svg]]

> [!tip]- Pista de arranque
>
> Convierte las distancias a metros. Calcula el campo de una sola masa con $g=GM/r^2$ y descompón cada vector. Por simetría, las componentes horizontales se anulan y las verticales se suman.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

### 2. Campo gravitatorio con masas en posiciones distintas — **R**

**Situación.** Se busca el campo en el origen debido a dos masas puntuales. Primero determina hacia dónde atrae cada masa; después suma las componentes con sus signos.

**Datos**

- $M_1=M_2=2.0\times10^{10}\,\mathrm{kg}$.
- Posiciones: $M_1=(-3.0,0)\,\mathrm{km}$ y $M_2=(0,4.0)\,\mathrm{km}$.
- Punto de cálculo: $O=(0,0)$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Encuentra $g_x$, $g_y$, $|\vec g|$ y el ángulo medido **al norte del oeste**.

![[imagenes/campo-no-simetrico.svg]]

> [!tip]- Pista de arranque
>
> Convierte cada posición a metros. En el origen, la contribución de $M_1$ apunta al oeste ($-x$) y la de $M_2$ al norte ($+y$). Calcula cada módulo por separado, suma componentes y usa $\tan\theta=|g_y/g_x|$.

### 3. Recuperar el peso en la superficie — **M**

**Situación.** Un satélite pesa menos a cierta altura porque está más lejos del centro terrestre. Se conoce su peso orbital y se quiere inferir cuánto pesaría en la superficie.

**Datos**

- Peso a la altura $h=0.35R_T$: $W_h=38\,\mathrm{kN}$.
- Radio terrestre: $R_T$.
- La masa del satélite no cambia.

**Se pide.** Calcula el peso superficial $W_0$.

![[imagenes/orbita-satelite.svg]]

> [!tip]- Pista de arranque
>
> La distancia al centro en órbita es $r=R_T+h=1.35R_T$. Como el peso es proporcional a $1/r^2$, forma el cociente $W_h/W_0=(R_T/r)^2$ y despeja $W_0$.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

### 4. Peso superficial y peso a 350 km — **R**

**Situación.** Una nave mantiene la misma masa al pasar de la superficie a una órbita baja. Compara su peso en ambos lugares.

**Datos**

- Masa: $m=4.20\times10^5\,\mathrm{kg}$.
- Altura: $h=350\,\mathrm{km}$.
- $R_T=6380\,\mathrm{km}$.
- $g_0=9.81\,\mathrm{m/s^2}$.

**Se pide.** Calcula $W_0$ en superficie y $W_h$ a esa altura.

![[imagenes/orbita-satelite.svg]]

> [!tip]- Pista de arranque
>
> En la superficie usa $W_0=mg_0$. Para la altura, calcula primero $r=R_T+h$ y luego $g(h)=g_0[R_T/(R_T+h)]^2$. Conserva unidades compatibles en el cociente.

### 5. Satélite lunar: rapidez, período, energía y escape — **M**

**Situación.** Un satélite está en órbita circular alrededor de la Luna. El radio dado es múltiplo del radio lunar: no es una altura sobre la superficie.

**Datos**

- Masa de la Luna: $M_L=7.35\times10^{22}\,\mathrm{kg}$.
- Radio lunar: $R_L=1.74\times10^6\,\mathrm{m}$.
- Masa del satélite: $m=500\,\mathrm{kg}$.
- Radio orbital desde el centro: $r=5R_L$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula rapidez orbital, período, energía mecánica total y rapidez de escape desde ese mismo radio.

![[imagenes/orbita-satelite.svg]]

> [!tip]- Pista de arranque
>
> Empieza por $r=5R_L$. Para la órbita circular iguala gravedad y fuerza centrípeta; luego usa $T=2\pi r/v$. La energía total de una órbita circular es $-GM_Lm/(2r)$. Para escapar desde $r$, exige energía final cero.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

### 6. Tercera ley de Kepler: distancia media de Marte — **M**

**Situación.** Marte y la Tierra orbitan el mismo cuerpo central. Usa la órbita terrestre como referencia para no necesitar la masa del Sol.

**Datos**

- Período de Marte: $T_M=1.87$ años terrestres.
- Período de la Tierra: $T_T=1.00$ año.
- Radio medio terrestre: $r_T=1.00\,\mathrm{UA}=1.496\times10^{11}\,\mathrm{m}$.

**Se pide.** Calcula $r_M$ en UA y en metros.

> [!tip]- Pista de arranque
>
> Para dos órbitas alrededor del mismo Sol, $T^2/r^3$ es constante. Despeja $r_M=r_T(T_M/T_T)^{2/3}$ y convierte las UA a metros al final.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

### 7. Inferir la masa del Sol a partir de la órbita terrestre — **M**

**Situación.** La gravedad del Sol proporciona la aceleración centrípeta de la Tierra. La masa terrestre aparece en ambos lados y se cancela.

**Datos**

- Radio orbital: $r=1.496\times10^{11}\,\mathrm{m}$.
- Período: $T=3.156\times10^7\,\mathrm{s}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula la masa solar $M_\odot$.

> [!tip]- Pista de arranque
>
> Iguala $GM_\odot m/r^2$ con $m4\pi^2r/T^2$. Cancela $m$, despeja $M_\odot$ y comprueba que la unidad final sea kg.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

## Clave breve

> [!example]- Clave breve — abrir solo después de intentar
>
> 1. $|\vec g|=2.08\times10^{-9}\,\mathrm{m/s^2}$, vertical hacia abajo; las componentes horizontales se cancelan.
> 2. $g_x=-1.48\times10^{-7}\,\mathrm{m/s^2}$; $g_y=+8.34\times10^{-8}\,\mathrm{m/s^2}$; $|\vec g|=1.70\times10^{-7}\,\mathrm{m/s^2}$; $29.3^\circ$ al norte del oeste.
> 3. $W_0=69.3\,\mathrm{kN}$.
> 4. $W_0=4.12\times10^6\,\mathrm{N}$; $W_h=3.70\times10^6\,\mathrm{N}$.
> 5. $v_{orb}=750.7\,\mathrm{m/s}$; $T=7.28\times10^4\,\mathrm{s}=20.2\,\mathrm{h}$; $E=-1.41\times10^8\,\mathrm{J}$; $v_{esc}=1.06\times10^3\,\mathrm{m/s}$.
> 6. $r_M=1.52\,\mathrm{UA}=2.27\times10^{11}\,\mathrm{m}$.
> 7. $M_\odot=1.99\times10^{30}\,\mathrm{kg}$.

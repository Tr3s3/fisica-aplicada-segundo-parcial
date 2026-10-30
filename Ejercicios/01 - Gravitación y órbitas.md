---
tags: [fisica-aplicada, ejercicios, gravitacion]
---

# Ejercicios — Gravitación y órbitas

**Teoría:** [[Teoría/01 - Gravitación y órbitas]] · **Resoluciones:** [[Resoluciones/01 - Gravitación y órbitas]] · **Método:** [[Ejercicios/00 - Método y registro]]

> [!info] Cómo usar esta hoja
> Se conserva la numeración global para que coincida con el plan. **M** reproduce un tipo de los modelos; **R** es una variante de entrenamiento; **C** identifica complementarios reescritos a partir del TP 5. Resuelve primero sin abrir la pista; consulta la clave al final. La prioridad estima cuánto conviene dedicarles según los modelos: alta, media o ampliación.

## Ejercicios del tema

### 1. Aceleración inicial por dos masas simétricas — **M**

**Situación.** Una esfera de prueba de $0.010\,\mathrm{kg}$ se suelta desde el reposo en $P$. Dos esferas iguales, fijas en $A$ y $B$, son las únicas que la atraen. Calcula su aceleración inicial; el campo que producen no depende de la masa de prueba.

**Datos**

- $M_1=M_2=0.260\,\mathrm{kg}$.
- Masa de la esfera de prueba: $m=0.010\,\mathrm{kg}$.
- Separación entre las masas: $16.0\,\mathrm{cm}$.
- $P$ está $6.0\,\mathrm{cm}$ arriba del punto medio y a $10.0\,\mathrm{cm}$ de cada masa.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula el módulo y la dirección de la aceleración inicial $\vec a(P)$.

![[imagenes/campo-gravitatorio.svg]]

Las flechas representan campos; las fuerzas sobre la esfera de prueba tienen los mismos sentidos.

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
- Masa del satélite: $m=5000\,\mathrm{kg}$, como indica el modelo 2025.
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

### 8. Fuerza neta y punto de fuerza nula en una línea — **R · TP 5, ejercicio 2**

**Situación.** Dos masas están fijas sobre una misma recta. Una tercera masa se coloca primero en el punto medio y luego se busca dónde las atracciones se equilibran.

**Datos**

- $M_1=200\,\mathrm{kg}$ y $M_2=500\,\mathrm{kg}$.
- Separación entre las masas: $d=4.0\,\mathrm{m}$.
- Masa de prueba: $m=50\,\mathrm{kg}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** a) Halla la fuerza neta sobre $m$ en el punto medio, con sentido. b) Encuentra la posición entre $M_1$ y $M_2$ donde la fuerza neta es cero, medida desde $M_1$.

> [!tip]- Pista de arranque
> En el punto medio las dos fuerzas son opuestas. Para el punto nulo, iguala sus módulos y deja $x$ como distancia desde $M_1$; no iguales las masas ni las distancias directamente.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

### 9. Gravedad efectiva en el ecuador de Júpiter — **R · TP 5, ejercicio 9**

**Situación.** La gravedad tira hacia el centro, pero una persona en el ecuador también necesita aceleración centrípeta por la rotación del planeta. La balanza ejerce una fuerza hacia afuera y su lectura corresponde al peso aparente.

![[imagenes/gravedad-rotacion-jupiter.svg]]

**Datos**

- $M_J=1.9\times10^{27}\,\mathrm{kg}$.
- Radio ecuatorial: $R_J=7.1\times10^4\,\mathrm{km}$.
- Período de rotación: $T_J=9\,\mathrm{h}\,55\,\mathrm{min}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$; usa $g_\oplus=9.80\,\mathrm{m/s^2}$ para expresar el resultado en unidades terrestres de $g$.

**Se pide.** Calcula la aceleración centrípeta, la gravedad efectiva que determina la lectura de la balanza y cuántas veces $g_\oplus$ representa.

> [!tip]- Pista de arranque
> Convierte $R_J$ a metros y $T_J$ a segundos. En el ecuador, hacia adentro es positivo: $mg-N=m v^2/R_J$. Despeja $N/m$.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

### 10. Energía y rapidez de un meteorito en caída — **R · TP 5, ejercicio 14**

**Situación.** Un meteorito se mueve radialmente hacia la Tierra. Sin atmósfera, la gravedad es conservativa: la pérdida de energía potencial se convierte en ganancia de energía cinética.

**Datos**

- Masa: $m=1.00\times10^3\,\mathrm{kg}$.
- Rapidez inicial: $v_i=100\,\mathrm{km/h}$ cuando $r_i=6R_\oplus$.
- Radio terrestre: $R_\oplus=6.38\times10^6\,\mathrm{m}$.
- Masa terrestre: $M_\oplus=5.97\times10^{24}\,\mathrm{kg}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula la energía potencial inicial y en la superficie, la rapidez justo antes de llegar a la superficie y el trabajo realizado por la gravedad. Se supone caída radial y se desprecia la atmósfera.

> [!tip]- Pista de arranque
> Usa $U=-GM_\oplus m/r$ con cero en el infinito. Para la rapidez, conserva $K+U$; el trabajo gravitatorio es $W_g=-\Delta U$.

**Para comparar después:** [[Resoluciones/01 - Gravitación y órbitas]].

## Complementarios del TP 5

Los complementarios amplían el alcance del TP sin desplazar los ejercicios que coinciden con los modelos de parcial. Empieza por prioridad alta; deja las ampliaciones para el final.

### C1. Fuerza entre las esferas de una balanza de Cavendish — **TP 5, ejercicio 1 · Prioridad media**

**Situación.** Una esfera pequeña y una grande se atraen mutuamente. Se modelan como masas puntuales separadas por la distancia entre sus centros.

**Datos**

- $m_1=0.010\,\mathrm{kg}$.
- $m_2=500\,\mathrm{g}$.
- Separación entre centros: $r=0.050\,\mathrm{m}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula el módulo de la fuerza gravitatoria que cada esfera ejerce sobre la otra e indica la relación entre sus direcciones.

> [!tip]- Pista de arranque
>
> Convierte primero $500\,\mathrm{g}$ a kilogramos. Aplica $F=Gm_1m_2/r^2$; por la tercera ley de Newton, las dos fuerzas tienen igual módulo y sentidos opuestos.

### C2. Fuerza sobre una estrella en un triángulo de 45° — **TP 5, ejercicio 4 · Prioridad alta**

**Situación.** Una estrella pequeña está en el origen. Dos estrellas grandes la atraen desde los vértices restantes de un triángulo rectángulo isósceles. El eje $+x$ apunta a la derecha y $+y$ hacia arriba.

![[imagenes/fuerzas-estrellas-triangulo.svg]]

**Datos**

- Estrella pequeña en $(0,0)$, masa $m=1.00\times10^{30}\,\mathrm{kg}$.
- Estrella $M_2$ en $(2.00\times10^{12},0)\,\mathrm{m}$, masa $8.00\times10^{30}\,\mathrm{kg}$.
- Estrella $M_1$ en $(2.00\times10^{12},2.00\times10^{12})\,\mathrm{m}$, masa $8.00\times10^{30}\,\mathrm{kg}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula las componentes de la fuerza total sobre la estrella pequeña, su módulo y su dirección medida desde $+x$ hacia $+y$.

> [!tip]- Pista de arranque
>
> Calcula por separado las fuerzas hacia $M_1$ y $M_2$. La primera está a $45^\circ$ y la segunda es horizontal; suma sus componentes, no sus módulos directamente.

### C3. Fuerza planetaria sobre la Tierra durante una alineación — **TP 5, ejercicio 5 · Ampliación**

**Situación.** En una alineación ideal, los planetas están ordenados en una misma recta como Sol–Venus–Tierra–Júpiter–Saturno. Calcula solo la fuerza gravitatoria ejercida por esos tres planetas sobre la Tierra; no incluyas la fuerza del Sol.

![[imagenes/planetas-alineados.svg]]

**Datos**

- $M_E=5.97\times10^{24}\,\mathrm{kg}$.
- $M_V=0.815M_E$, $M_J=318M_E$, $M_{Sat}=95.1M_E$.
- Distancias medias al Sol: Venus $108$, Tierra $150$, Júpiter $778$ y Saturno $1430$ millones de km.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Encuentra las distancias entre la Tierra y cada planeta, calcula las tres fuerzas con signo sobre un eje positivo alejándose del Sol y determina la fuerza resultante.

> [!tip]- Pista de arranque
>
> Resta las distancias heliocéntricas para obtener $42$, $628$ y $1280$ millones de km. Venus atrae hacia el Sol; Júpiter y Saturno atraen en sentido contrario. Convierte cada distancia a metros antes de usar la ley de gravitación.

### C4. De un peso en Marte a pesos en la Tierra — **TP 5, ejercicio 6 · Prioridad alta (a–c); ampliación (d)**

**Situación.** Una persona pesa $45\,\mathrm{N}$ sobre la superficie de Marte. Se supone que las expresiones de campo de una esfera se aplican fuera de ella. Para la última parte, calcula únicamente la fuerza del Sol sobre la persona situada a una distancia de una unidad astronómica.

**Datos**

- $M_M=0.107M_E$, $R_M=3.36\times10^6\,\mathrm{m}$.
- $M_E=5.97\times10^{24}\,\mathrm{kg}$, $R_E=6.38\times10^6\,\mathrm{m}$.
- Peso en Marte: $W_M=45\,\mathrm{N}$.
- Altura sobre la superficie terrestre: $h=500\,\mathrm{km}$.
- Para la fuerza solar: $M_\odot=1.99\times10^{30}\,\mathrm{kg}$ y distancia Tierra–Sol $d=1.496\times10^{11}\,\mathrm{m}$.
- $g_0=9.81\,\mathrm{m/s^2}$, $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** a) Calcula la masa de la persona y explica si cambia al trasladarla. b) Calcula su peso en la superficie terrestre. c) Calcula su peso a $500\,\mathrm{km}$ de altura. d) Calcula por separado la fuerza gravitatoria del Sol sobre ella en la órbita terrestre.

> [!tip]- Pista de arranque
>
> Halla primero $g_M=GM_M/R_M^2$ y usa $m=W_M/g_M$. La masa permanece igual; para el peso a altura usa $r=R_E+h$. En la parte d aplica $F=GM_\odot m/d^2$; esa fuerza no es el peso que marca una balanza.

### C5. Cómo cambia la gravedad al cambiar masa y radio — **TP 5, ejercicios 7 y 8 · Prioridad media**

**Situación.** Compara la aceleración gravitatoria en la superficie de planetas esféricos con la de la Tierra.

**Se pide.** a) Un planeta tiene la misma masa que la Tierra y un radio $2.3R_E$. Calcula su $g$ si $g_E=9.81\,\mathrm{m/s^2}$. b) Si la masa de otro planeta se duplica y su radio se triplica, ¿por qué factor cambia su gravedad superficial?

> [!tip]- Pista de arranque
>
> Parte de $g=GM/R^2$. En cada caso forma el cociente $g'/g_E$ o $g'/g$ antes de sustituir; así se cancelan las constantes que no cambian.

### C6. Período orbital de Neptuno — **TP 5, ejercicio 11 · Prioridad alta**

**Situación.** Neptuno y la Tierra orbitan el Sol. Usa la Tierra como referencia y supone órbitas circulares para aplicar la misma relación de Kepler.

**Datos**

- Distancia media Neptuno–Sol: $r_N=4.5\times10^9\,\mathrm{km}$.
- Distancia media Tierra–Sol: $r_E=1.50\times10^8\,\mathrm{km}$.
- Período terrestre: $T_E=1.00\,\mathrm{año}$.

**Se pide.** Estima el período orbital de Neptuno en años terrestres.

> [!tip]- Pista de arranque
>
> Usa $T_N/T_E=(r_N/r_E)^{3/2}$. Las distancias pueden permanecer en kilómetros porque aparecen en un cociente; calcula ese cociente antes de elevarlo.

### C7. Satélite: órbita y energía necesaria para escapar — **TP 5, ejercicio 13 · Prioridad alta**

**Situación.** Un satélite de masa $m$ recorre una órbita circular alrededor de un planeta. La energía que se pide es el aumento mínimo de energía mecánica para pasar desde esa órbita hasta el infinito con rapidez final nula.

**Datos**

- $m=5000\,\mathrm{kg}$.
- Masa del planeta: $M=2.2\times10^{24}\,\mathrm{kg}$.
- Radio orbital medido desde el centro: $r=30000\,\mathrm{km}$.
- $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$.

**Se pide.** Calcula el período, la rapidez orbital, la rapidez de escape desde ese radio y el aumento mínimo de energía mecánica necesario para escapar desde la órbita circular.

> [!tip]- Pista de arranque
>
> Convierte $r$ a metros. Usa $v_{orb}=\sqrt{GM/r}$, $T=2\pi\sqrt{r^3/(GM)}$ y $v_{esc}=\sqrt{2GM/r}$. La energía orbital inicial es $-GMm/(2r)$; llevarla a cero requiere una energía positiva de igual módulo.

### C8. Por qué una caída corta da $v\approx\sqrt{2gh}$ — **TP 5, ejercicio 15 · Ampliación**

**Situación.** Un cuerpo se suelta desde el reposo a una altura $h$ sobre la superficie terrestre. Se desprecia la resistencia del aire. Cuando $h\ll R_E$, la gravedad varía muy poco durante la caída.

**Se pide.** Partiendo de la conservación de la energía gravitatoria, demuestra que la rapidez al llegar al suelo se aproxima por $v\approx\sqrt{2gh}$, donde $g=GM_E/R_E^2$ es la gravedad superficial.

> [!tip]- Pista de arranque
>
> Escribe la energía potencial inicial a $R_E+h$ y la final a $R_E$. Simplifica la diferencia exacta y luego usa $R_E+h\approx R_E$, válido cuando $h/R_E$ es pequeño.

## Clave breve

> [!example]- Clave breve — abrir solo después de intentar
>
> 1. $|\vec a|=2.08\times10^{-9}\,\mathrm{m/s^2}$, vertical hacia abajo; las componentes horizontales se cancelan.
> 2. $g_x=-1.48\times10^{-7}\,\mathrm{m/s^2}$; $g_y=+8.34\times10^{-8}\,\mathrm{m/s^2}$; $|\vec g|=1.70\times10^{-7}\,\mathrm{m/s^2}$; $29.4^\circ$ al norte del oeste.
> 3. $W_0=69.3\,\mathrm{kN}$.
> 4. $W_0=4.12\times10^6\,\mathrm{N}$; $W_h=3.70\times10^6\,\mathrm{N}$.
> 5. $v_{orb}=750.7\,\mathrm{m/s}$; $T=7.28\times10^4\,\mathrm{s}=20.2\,\mathrm{h}$; $E=-1.41\times10^9\,\mathrm{J}$; $v_{esc}=1.06\times10^3\,\mathrm{m/s}$.
> 6. $r_M=1.52\,\mathrm{UA}=2.27\times10^{11}\,\mathrm{m}$.
> 7. $M_\odot=1.99\times10^{30}\,\mathrm{kg}$.
> 8. En el punto medio, $F_{net}=2.50\times10^{-7}\,\mathrm{N}$ hacia $M_2$; el punto nulo está a $1.55\,\mathrm{m}$ de $M_1$.
> 9. $a_c=2.20\,\mathrm{m/s^2}$; $g_{ef}=22.9\,\mathrm{m/s^2}=2.34g_\oplus$.
> 10. $U_i=-1.04\times10^{10}\,\mathrm{J}$; $U_f=-6.24\times10^{10}\,\mathrm{J}$; $v_f=1.02\times10^4\,\mathrm{m/s}$; $W_g=+5.20\times10^{10}\,\mathrm{J}$.
> C1. $F=1.33\times10^{-10}\,\mathrm{N}$ sobre cada esfera; sentidos opuestos.
> C2. $F_x=1.81\times10^{26}\,\mathrm{N}$; $F_y=4.72\times10^{25}\,\mathrm{N}$; $|\vec F|=1.87\times10^{26}\,\mathrm{N}$ a $14.6^\circ$ sobre $+x$.
> C3. $F_V=1.10\times10^{18}\,\mathrm{N}$ hacia el Sol; $F_J=1.92\times10^{18}\,\mathrm{N}$ y $F_{Sat}=1.38\times10^{17}\,\mathrm{N}$ alejándose del Sol; resultante $9.56\times10^{17}\,\mathrm{N}$ alejándose del Sol.
> C4. $m=11.9\,\mathrm{kg}$; $W_E=117\,\mathrm{N}$; $W_{500\,km}=101\,\mathrm{N}$; $F_\odot=7.07\times10^{-2}\,\mathrm{N}$ hacia el Sol.
> C5. a) $g'=1.85\,\mathrm{m/s^2}$. b) $g'/g=2/9$.
> C6. $T_N\approx164\,\mathrm{años}$.
> C7. $T=8.52\times10^4\,\mathrm{s}=23.7\,\mathrm{h}$; $v_{orb}=2.21\times10^3\,\mathrm{m/s}$; $v_{esc}=3.13\times10^3\,\mathrm{m/s}$; $\Delta E=1.22\times10^{10}\,\mathrm{J}$.
> C8. $v=\sqrt{2GM_Eh/[R_E(R_E+h)]}\approx\sqrt{2GM_Eh/R_E^2}=\sqrt{2gh}$ cuando $h\ll R_E$.

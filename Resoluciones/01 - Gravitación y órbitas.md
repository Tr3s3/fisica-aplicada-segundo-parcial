---
tags: [fisica-aplicada, resoluciones, gravitacion]
---

# Resoluciones completas — Gravitación y órbitas

**Recorrido:** [[Teoría/01 - Conceptos de gravitación y órbitas|Conceptos]] · [[Teoría/01 - Fórmulas aplicadas de gravitación y órbitas|Fórmulas]] · [[Ejercicios/01 - Gravitación y órbitas|Enunciados y pistas]]

> [!info] Método
> Antes de mirar cada sección, intenta dibujar el sistema y elegir la ley que conecta los datos con lo pedido. Se conserva la numeración global del banco.

## 1. Aceleración inicial por dos masas simétricas

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

![[imagenes/campo-gravitatorio.svg]]

### Interpretar la geometría

Las masas están a $8.0\,\mathrm{cm}$ a cada lado del eje vertical, pues su separación total es $16.0\,\mathrm{cm}$. El punto $P$ está $6.0\,\mathrm{cm}$ arriba del punto medio. La distancia diagonal es $10.0\,\mathrm{cm}$, como confirma el triángulo $6$-$8$-$10$. La esfera de prueba tiene masa $m=0.010\,\mathrm{kg}$ y se suelta desde el reposo.

### Calcular el campo de una masa

$$
r=10.0\,\mathrm{cm}=0.100\,\mathrm{m},
\qquad
g_1=\frac{GM}{r^2}
=\frac{(6.67\times10^{-11})(0.260)}{(0.100)^2}
=1.734\times10^{-9}\,\mathrm{m/s^2}.
$$

La masa de prueba no aparece porque buscamos campo, no fuerza sobre una masa específica.

### Separar componentes y usar simetría

La componente vertical de cada campo es $g_1(6/10)$. Las componentes horizontales tienen igual módulo y sentidos contrarios:

$$
g_x=0,\qquad
g_y=-2g_1\frac{6}{10}.
$$

El signo negativo indica que la resultante apunta hacia abajo si $+y$ es hacia arriba.

### Pasar del campo a la aceleración

La fuerza neta sobre la esfera de prueba es $\vec F_{net}=m\vec g$. Por la segunda ley de Newton,

$$
\vec a=\frac{\vec F_{net}}{m}=\vec g.
$$

Si se desea comprobar la fuerza primero, $F_{net}=0.010(2.08\times10^{-9})=2.08\times10^{-11}\,\mathrm{N}$.

### Resultado y control

$$
\vec g(P)=\vec a(P)=-2.08\times10^{-9}\,\hat y\,\mathrm{m/s^2},
\qquad
|\vec a|=2.08\times10^{-9}\,\mathrm{m/s^2}.
$$

La aceleración inicial es vertical hacia abajo, es decir, hacia las dos masas. El módulo es menor que la suma de los dos módulos completos, pues solo se suman las componentes verticales.

## 2. Campo de masas en posiciones distintas

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

![[imagenes/campo-no-simetrico.svg]]

### Definir ejes y direcciones

Tomamos $+x$ hacia el este y $+y$ hacia el norte. El punto de cálculo es el origen.

- $M_1$, al oeste, produce campo hacia el oeste: componente $x$ negativa.
- $M_2$, al norte, produce campo hacia el norte: componente $y$ positiva.

Esta asignación de signos se hace antes del cálculo porque la gravedad atrae a cada masa fuente.

### Convertir las distancias

$$
r_1=3.0\,\mathrm{km}=3.00\times10^3\,\mathrm{m},
\qquad
r_2=4.0\,\mathrm{km}=4.00\times10^3\,\mathrm{m}.
$$

### Calcular cada campo

$$
g_1=\frac{GM_1}{r_1^2}
=\frac{(6.67\times10^{-11})(2.0\times10^{10})}{(3.00\times10^3)^2}
=1.48\times10^{-7}\,\mathrm{m/s^2},
$$

$$
g_2=\frac{GM_2}{r_2^2}
=\frac{(6.67\times10^{-11})(2.0\times10^{10})}{(4.00\times10^3)^2}
=8.34\times10^{-8}\,\mathrm{m/s^2}.
$$

Los campos son perpendiculares, así que sus módulos se asignan directamente a las componentes con los signos definidos:

$$
g_x=-1.48\times10^{-7}\,\mathrm{m/s^2},
\qquad
g_y=+8.34\times10^{-8}\,\mathrm{m/s^2}.
$$

### Hallar módulo y ángulo

$$
|\vec g|=\sqrt{g_x^2+g_y^2}
=1.70\times10^{-7}\,\mathrm{m/s^2}.
$$

El ángulo agudo desde el oeste hacia el norte satisface

$$
\tan\theta=\frac{|g_y|}{|g_x|},
\qquad
\theta=29.4^\circ.
$$

**Respuesta:** $1.70\times10^{-7}\,\mathrm{m/s^2}$, a $29.4^\circ$ al norte del oeste. Los signos $g_x<0$, $g_y>0$ confirman el cuadrante noroeste.

## 3. Recuperar el peso superficial desde el peso orbital

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

### Relacionar altura con radio

$h=0.35R_T$, por tanto la distancia al centro terrestre es

$$
r=R_T+h=1.35R_T.
$$

Para el mismo satélite, $W\propto1/r^2$. Entonces,

$$
\frac{W_h}{W_0}
=\left(\frac{R_T}{1.35R_T}\right)^2
=\frac{1}{1.35^2}.
$$

### Despejar y calcular

$$
W_0=W_h(1.35)^2
=(38\,\mathrm{kN})(1.8225)
=69.255\,\mathrm{kN}.
$$

Con tres cifras significativas,

$$
\boxed{W_0=69.3\,\mathrm{kN}}.
$$

El peso superficial debe ser mayor que $38\,\mathrm{kN}$, pues en superficie la distancia al centro es menor. No hace falta hallar la masa.

## 4. Peso en superficie y a 350 km

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

![[imagenes/orbita-satelite.svg]]

### Convertir datos y hallar el radio orbital

$$
m=4.20\times10^5\,\mathrm{kg},\quad
R_T=6380\,\mathrm{km}=6.380\times10^6\,\mathrm{m},\quad
h=350\,\mathrm{km}=3.50\times10^5\,\mathrm{m}.
$$

La distancia al centro es

$$
r=R_T+h=6.730\times10^6\,\mathrm{m}.
$$

Se suma $R_T+h$ porque la gravedad depende de la distancia al centro terrestre.

### Peso superficial

$$
W_0=mg_0
=(4.20\times10^5)(9.81)
=4.1202\times10^6\,\mathrm{N}.
$$

### Gravedad y peso a 350 km

Al dividir $g(h)=GM_T/r^2$ por $g_0=GM_T/R_T^2$, se cancelan $G$ y $M_T$:

$$
g(h)=g_0\left(\frac{R_T}{R_T+h}\right)^2
=(9.81)\left(\frac{6380}{6730}\right)^2
=8.82\,\mathrm{m/s^2}.
$$

Por tanto,

$$
W_h=mg(h)
=(4.20\times10^5)(8.82)
\approx3.70\times10^6\,\mathrm{N}.
$$

**Respuesta:** $W_0=4.12\times10^6\,\mathrm{N}$, $W_h=3.70\times10^6\,\mathrm{N}$. La masa no cambia; el peso orbital es menor.

## 5. Satélite lunar: rapidez, período, energía y escape

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

![[imagenes/orbita-satelite.svg]]

### Radio orbital

El satélite tiene masa $m=5000\,\mathrm{kg}$, dato necesario para calcular la energía total. El dato $5R_L$ ya es un radio medido desde el centro lunar:

$$
r=5R_L=5(1.74\times10^6\,\mathrm{m})
=8.70\times10^6\,\mathrm{m}.
$$

No se suma otro $R_L$.

### Rapidez orbital circular

La gravedad proporciona la aceleración centrípeta. Igualar $GM_Lm/r^2=mv^2/r$ y cancelar la masa del satélite produce

$$
v_{\mathrm{orb}}=\sqrt{\frac{GM_L}{r}}
=\sqrt{\frac{(6.67\times10^{-11})(7.35\times10^{22})}{8.70\times10^6}}
=750.7\,\mathrm{m/s}.
$$

### Período

Una vuelta recorre $2\pi r$:

$$
T=\frac{2\pi r}{v_{\mathrm{orb}}}
=\frac{2\pi(8.70\times10^6)}{750.7}
=7.282\times10^4\,\mathrm{s}
=20.2\,\mathrm{h}.
$$

La división por $3600\,\mathrm{s/h}$ convierte segundos a horas.

### Energía total

En órbita circular $K=GM_Lm/(2r)$ y $U=-GM_Lm/r$. Al sumar,

$$
E=K+U=-\frac{GM_Lm}{2r}
=-\frac{(6.67\times10^{-11})(7.35\times10^{22})(5000)}{2(8.70\times10^6)}
=-1.41\times10^9\,\mathrm{J}.
$$

Es negativa porque el satélite está ligado a la Luna; hay que aportarle energía para llevarlo al infinito.

### Rapidez de escape desde ese radio

La rapidez límite deja energía final nula en el infinito:

$$
\frac12m v_{\mathrm{esc}}^2-\frac{GM_Lm}{r}=0
\quad\Rightarrow\quad
v_{\mathrm{esc}}=\sqrt{\frac{2GM_L}{r}}
=1.062\times10^3\,\mathrm{m/s}.
$$

**Respuesta:** $v_{\mathrm{orb}}=750.7\,\mathrm{m/s}$, $T=20.2\,\mathrm{h}$, $E=-1.41\times10^9\,\mathrm{J}$, $v_{\mathrm{esc}}=1.06\times10^3\,\mathrm{m/s}$.

> [!warning] Interpretación
> Es la rapidez total requerida por la definición usual de escape desde el radio indicado. No es automáticamente el incremento que debe recibir un satélite que ya viaja a rapidez orbital.

## 6. Distancia media de Marte por Kepler

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

Marte y la Tierra orbitan el mismo Sol, por lo que $T^2/r^3$ es igual para ambos:

$$
\frac{T_M^2}{r_M^3}
=\frac{T_T^2}{r_T^3}.
$$

Despejamos el radio de Marte:

$$
r_M=r_T\left(\frac{T_M}{T_T}\right)^{2/3}.
$$

Usando la órbita terrestre como referencia,

$$
r_M=(1.00\,\mathrm{UA})
\left(\frac{1.87\,\mathrm{años}}{1.00\,\mathrm{año}}\right)^{2/3}
=1.518\,\mathrm{UA}.
$$

Los años se cancelan en el cociente. El período de Marte es mayor, así que su radio debe superar $1\,\mathrm{UA}$.

$$
r_M=(1.518)(1.496\times10^{11}\,\mathrm{m})
=2.27\times10^{11}\,\mathrm{m}.
$$

**Respuesta:** $1.52\,\mathrm{UA}=2.27\times10^{11}\,\mathrm{m}$.

## 7. Masa solar desde la órbita terrestre

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]]

### Relacionar gravedad y movimiento circular

La rapidez en una órbita circular es $v=2\pi r/T$; por ello la aceleración centrípeta es

$$
a_c=\frac{v^2}{r}
=\frac{4\pi^2r}{T^2}.
$$

La gravedad solar proporciona esa aceleración:

$$
\frac{GM_\odot m_T}{r^2}
=m_T\frac{4\pi^2r}{T^2}.
$$

### Cancelar la masa terrestre y despejar

La masa terrestre aparece en ambos lados y se cancela:

$$
\frac{GM_\odot}{r^2}
=\frac{4\pi^2r}{T^2}
\quad\Rightarrow\quad
M_\odot=\frac{4\pi^2r^3}{GT^2}.
$$

### Sustituir en SI

$$
M_\odot=
\frac{4\pi^2(1.496\times10^{11}\,\mathrm{m})^3}
{(6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2})(3.156\times10^7\,\mathrm{s})^2}
=1.99\times10^{30}\,\mathrm{kg}.
$$

La unidad resultante es kg. El orden de magnitud, alrededor de $10^{30}\,\mathrm{kg}$, es consistente con una masa estelar.

## 8. Fuerza neta y posición de fuerza nula

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]] · TP 5, ejercicio 2.

Tomamos el eje $x$ sobre la línea de las masas, con $M_1=200\,\mathrm{kg}$ en $x=0$ y $M_2=500\,\mathrm{kg}$ en $x=4.0\,\mathrm{m}$. La masa de prueba está en el punto medio, $x=2.0\,\mathrm{m}$.

### a) Fuerza neta en el punto medio

Las dos fuerzas tienen la misma distancia, pero sentidos opuestos. La fuerza de $M_1$ apunta a la izquierda y la de $M_2$ a la derecha:

$$
F_1=G\frac{M_1m}{(2.0)^2}
=1.67\times10^{-7}\,\mathrm{N},
\qquad
F_2=G\frac{M_2m}{(2.0)^2}
=4.17\times10^{-7}\,\mathrm{N}.
$$

Elegimos a la derecha como sentido positivo:

$$
F_{net}=F_2-F_1
=2.50\times10^{-7}\,\mathrm{N}.
$$

La fuerza neta apunta hacia la masa de $500\,\mathrm{kg}$.

### b) Posición donde el campo y la fuerza se anulan

Sea $x$ la distancia desde $M_1$ hasta el punto buscado, dentro del segmento. Allí las fuerzas son opuestas. Para que se cancelen, sus módulos deben ser iguales:

$$
G\frac{M_1m}{x^2}
=G\frac{M_2m}{(4.0-x)^2}.
$$

Se cancelan $G$ y $m$. Al tomar la raíz positiva y despejar,

$$
\frac{4.0-x}{x}=\sqrt{\frac{M_2}{M_1}},
\qquad
x=\frac{4.0}{1+\sqrt{500/200}}
=1.55\,\mathrm{m}.
$$

El punto está a $1.55\,\mathrm{m}$ de $M_1$ y a $2.45\,\mathrm{m}$ de $M_2$. Queda más cerca de la masa menor: necesita estar más cerca para que su atracción iguale la de la masa mayor. Fuera del segmento, ambas fuerzas apuntan al mismo lado, así que no pueden anularse.

## 9. Gravedad efectiva en el ecuador de Júpiter

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]] · TP 5, ejercicio 9.

![[imagenes/gravedad-rotacion-jupiter.svg]]

### Convertir y calcular la gravedad newtoniana

$$
R_J=7.1\times10^4\,\mathrm{km}=7.1\times10^7\,\mathrm{m},
\qquad
T_J=9(3600)+55(60)=35700\,\mathrm{s}.
$$

La atracción gravitatoria por unidad de masa en la superficie es

$$
g_J=\frac{GM_J}{R_J^2}
=\frac{(6.67\times10^{-11})(1.9\times10^{27})}{(7.1\times10^7)^2}
=25.14\,\mathrm{m/s^2}.
$$

### Descontar lo necesario para la aceleración centrípeta

Una persona en reposo respecto de Júpiter rota con el planeta. En el ecuador su aceleración centrípeta apunta hacia el centro:

$$
a_c=\frac{4\pi^2R_J}{T_J^2}
=\frac{4\pi^2(7.1\times10^7)}{(35700)^2}
=2.20\,\mathrm{m/s^2}.
$$

La gravedad apunta hacia adentro y la fuerza normal de la balanza hacia afuera. La segunda ley radial es $mg_J-N=ma_c$, de modo que la lectura por unidad de masa es

$$
g_{ef}=\frac{N}{m}=g_J-a_c
=25.14-2.20
=22.94\,\mathrm{m/s^2}.
$$

En unidades del valor terrestre,

$$
\frac{g_{ef}}{g_\oplus}
=\frac{22.94}{9.80}
=2.34.
$$

**Respuesta:** la persona experimentaría un peso aparente equivalente a $2.34$ veces su peso terrestre. La rotación reduce la lectura respecto de $g_J$; no cambia la atracción gravitatoria $GM_J/R_J^2$.

## 10. Energía y rapidez de un meteorito en caída

**Enunciado:** [[Ejercicios/01 - Gravitación y órbitas]] · variante numérica del TP 5, ejercicio 14.

### Definir los estados y convertir la rapidez

El estado inicial está a $r_i=6R_\oplus$ y el final justo antes de tocar la superficie está a $r_f=R_\oplus$:

$$
r_i=6(6.38\times10^6)=3.828\times10^7\,\mathrm{m},
\qquad
v_i=100\,\mathrm{km/h}=27.78\,\mathrm{m/s}.
$$

### Calcular las energías potenciales

Se toma $U=0$ en el infinito, por eso $U=-GM_\oplus m/r$:

$$
U_i=-\frac{GM_\oplus m}{r_i}
=-\frac{(6.67\times10^{-11})(5.97\times10^{24})(1.00\times10^3)}{3.828\times10^7}
=-1.04\times10^{10}\,\mathrm{J},
\qquad
U_f=-\frac{GM_\oplus m}{R_\oplus}
=-\frac{(6.67\times10^{-11})(5.97\times10^{24})(1.00\times10^3)}{6.38\times10^6}
=-6.24\times10^{10}\,\mathrm{J}.
$$

La energía potencial disminuye: la gravedad hace trabajo positivo al acercar el meteorito.

### Usar conservación de la energía para hallar la rapidez

Como solo actúa la gravedad, $K_i+U_i=K_f+U_f$:

$$
\frac12mv_f^2=\frac12mv_i^2+(U_i-U_f),
\qquad
v_f=\sqrt{(27.78)^2+2(6.67\times10^{-11})(5.97\times10^{24})
\left(\frac1{6.38\times10^6}-\frac1{3.828\times10^7}\right)}
=1.02\times10^4\,\mathrm{m/s}.
$$

La masa se cancela en la ecuación de rapidez, aunque se necesita para dar $U$ y $W$ en joules.

### Obtener el trabajo de la gravedad

Para una fuerza conservativa, $W_g=-\Delta U$:

$$
W_g=-(U_f-U_i)
=U_i-U_f
=+5.20\times10^{10}\,\mathrm{J}.
$$

El signo positivo indica que la gravedad transfiere energía al movimiento durante la caída. El valor coincide con $K_f-K_i$ dentro del redondeo.

**Respuesta:** $U_i=-1.04\times10^{10}\,\mathrm{J}$, $U_f=-6.24\times10^{10}\,\mathrm{J}$, $v_f=1.02\times10^4\,\mathrm{m/s}$ y $W_g=+5.20\times10^{10}\,\mathrm{J}$.

## Idea decisiva por ejercicio

| Ejercicio | Principio físico |
|---:|---|
| 1–2 | Campo de cada fuente y suma vectorial |
| 3–4 | Inverso del cuadrado y distancia $R+h$ |
| 5 | Órbita circular, período, energía total y escape |
| 6 | Constante de Kepler común para planetas alrededor del mismo Sol |
| 7 | Fuerza gravitatoria igual a masa por aceleración centrípeta |
| 8 | Superposición de fuerzas en una dimensión y punto nulo |
| 9 | Segunda ley radial en un sistema que rota; peso aparente |
| 10 | Conservación de energía y trabajo de una fuerza conservativa |

## Fuentes y correspondencia con la cátedra

- [Capítulo 12: Gravitación](zotero://select/library/items/ATATDN6I): fuerza y superposición, PDF pp. 2–5; peso y dependencia con $r$, pp. 6–8; energía potencial y escape, pp. 8–10; órbitas, período y energía circular, pp. 12–13; Kepler, pp. 15–17.
- [TP 5 de Física Aplicada 2025](zotero://select/library/items/F4BGIQ83): ejercicios 2, 3, 6, 9, 10, 13 y 14 fundamentan los tipos de práctica 1–10. En el ejercicio 10 se agregó una masa explícita para que las energías y el trabajo puedan expresarse numéricamente.
- [Modelo del segundo parcial 2025, Tema A](zotero://select/library/items/6GRRT3TK), escaneo pp. 1–2: ejercicios 1 y 2 respaldan los enunciados M de aceleración por dos masas y satélite lunar. El satélite tiene masa $5000\,\mathrm{kg}$; el cambio de la energía total de esta guía a $-1.41\times10^9\,\mathrm{J}$ corrige una cifra que había quedado diez veces menor.

Las resoluciones explican los modelos ideales utilizados y los pasos de cálculo; las variantes R amplían los formatos de la guía de trabajos prácticos, sin atribuirlas al parcial.

---
tags: [fisica-aplicada, resoluciones, gravitacion]
---

# Resoluciones modelo — Gravitación y órbitas

Lee cada resolución con lápiz y papel: pausa antes del despeje, predice el siguiente paso y justifica por qué aplica esa ley. Para practicar primero, usa [[Ejercicios/01 - Gravitación y órbitas]].

**Teoría relacionada:** [[Teoría/01 - Gravitación y órbitas]]

---

## Peso a 350 km y masa constante

![[imagenes/orbita-satelite.svg]]

Datos de la resolución 2024: $h=350\,\mathrm{km}$, peso orbital $W_h=3.80\times10^6\,\mathrm N$, $R_T=6380\,\mathrm{km}$, $M_T=5.97\times10^{24}\,\mathrm{kg}$.

**1. Distancia al centro:** $r=R_T+h=6730\,\mathrm{km}=6.73\times10^6\,\mathrm m$.

**2. Gravedad a esa altura:**
$$
g(h)=\frac{GM_T}{r^2}
=\frac{(6.67\times10^{-11})(5.97\times10^{24})}{(6.73\times10^6)^2}
=8.79\,\mathrm{m/s^2}.
$$

**3. Masa:** $W_h=mg(h)$, entonces
$$
m=\frac{3.80\times10^6}{8.79}
=4.32\times10^5\,\mathrm{kg}.
$$
La masa no cambia al volver a la superficie. Con $g_0=9.81\,\mathrm{m/s^2}$:
$$
W_0=mg_0=(4.32\times10^5)(9.81)
=4.24\times10^6\,\mathrm N.
$$
El peso superficial supera al orbital porque la Tierra atrae más cerca de su superficie.

## Dos masas: aceleración gravitatoria vectorial

![[imagenes/campo-gravitatorio.svg]]

En el modelo PDF 2025, dos masas de $0.260\,\mathrm{kg}$ están simétricas respecto del eje vertical. El punto $P$ queda a $6.0\,\mathrm{cm}$ sobre el punto medio; cada masa está a $8.0\,\mathrm{cm}$ horizontalmente del eje y a $10.0\,\mathrm{cm}$ de $P$. En $P$ se suelta una masa de prueba de $0.010\,\mathrm{kg}$.

**1. Aceleración producida por una esfera:** la masa de prueba se cancela entre $F=mg$ y $F=GMm/r^2$:
$$
g_1=\frac{G M}{r^2}
=\frac{(6.67\times10^{-11})(0.260)}{(0.100)^2}
=1.734\times10^{-9}\,\mathrm{m/s^2}.
$$

**2. Componentes:** el triángulo es 6–8–10. La componente vertical de cada aceleración es $g_1(6/10)$. Las horizontales tienen sentidos opuestos y se cancelan.

**3. Suma vertical:** ambas apuntan hacia abajo:
$$
g_{net}=2g_1\frac{6}{10}
=2.08\times10^{-9}\,\mathrm{m/s^2}.
$$
Resultado: aceleración vertical hacia el punto medio entre las esferas. La masa de prueba no modifica este resultado.

## Satélite en órbita lunar: período, energía y escape

Datos del modelo PDF 2025: $M_L=7.35\times10^{22}\,\mathrm{kg}$, $R_L=1.74\times10^6\,\mathrm m$, $m=500\,\mathrm{kg}$, radio orbital $r=5R_L$.

**1. Radio orbital:** $r=5(1.74\times10^6)=8.70\times10^6\,\mathrm m$.

**2. Rapidez orbital:** igualamos gravedad y fuerza centrípeta, se cancela $m$:
$$
v_{orb}=\sqrt{\frac{GM_L}{r}}
=750.7\,\mathrm{m/s}.
$$

**3. Período:** $T=2\pi r/v_{orb}$:
$$
T=2\pi\sqrt{\frac{r^3}{GM_L}}
=7.282\times10^4\,\mathrm s
=20.23\,\mathrm h.
$$

**4. Energía total:** para órbita circular $K=GM_Lm/(2r)$ y $U=-GM_Lm/r$:
$$
E=K+U=-\frac{GM_Lm}{2r}
=-1.41\times10^8\,\mathrm J.
$$
Es negativa porque el satélite está ligado gravitatoriamente.

**5. Escape desde la órbita actual:** imponemos energía final cero:
$$
v_{esc}(r)=\sqrt{\frac{2GM_L}{r}}
=1.062\times10^3\,\mathrm{m/s}.
$$
Si el problema preguntara por escape desde la superficie lunar, se usaría $r=R_L$ y resultaría $2.37\times10^3\,\mathrm{m/s}$.

## Peso de lanzamiento desde el peso orbital

El modelo DOCX 2025 da $W_h=38\,\mathrm{kN}$ a una altura $h=0.35R_T$ y pide el peso en superficie.

**1. Radio desde el centro:** $r=R_T+h=1.35R_T$.

**2. Escala del peso:** $W_h/W_0=(R_T/r)^2$. Despejamos:
$$
W_0=W_h\left(\frac{r}{R_T}\right)^2
=(38\,\mathrm{kN})(1.35)^2
=69.3\,\mathrm{kN}.
$$
La gravedad superficial es mayor, por eso el mismo satélite pesa más al lanzamiento. No es necesario hallar su masa.

## Kepler: distancia de Marte y masa del Sol

### a) Distancia de Marte

Para la Tierra y Marte alrededor del Sol, $T^2/r^3$ es igual:
$$
r_M=r_T\left(\frac{T_M}{T_T}\right)^{2/3}
=(1\,\mathrm{UA})(1.87)^{2/3}
=1.518\,\mathrm{UA}.
$$
Con $1\,\mathrm{UA}=1.496\times10^{11}\,\mathrm m$:
$$
r_M=(1.518)(1.496\times10^{11})
=2.27\times10^{11}\,\mathrm m.
$$
El período mayor implica una órbita más grande.

### b) Masa del Sol

La fuerza gravitatoria proporciona la aceleración centrípeta de la Tierra:
$$
\frac{GM_\odot m}{r^2}
=m\frac{4\pi^2r}{T^2}
\quad\Rightarrow\quad
M_\odot=\frac{4\pi^2r^3}{GT^2}.
$$
Con $r=1.496\times10^{11}\,\mathrm m$, $T=3.156\times10^7\,\mathrm s$ y $G=6.67\times10^{-11}$:
$$
M_\odot=
\frac{4\pi^2(1.496\times10^{11})^3}
{(6.67\times10^{-11})(3.156\times10^7)^2}
=1.99\times10^{30}\,\mathrm{kg}.
$$

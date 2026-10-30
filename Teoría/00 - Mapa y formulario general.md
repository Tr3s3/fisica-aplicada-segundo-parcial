---
tags: [fisica-aplicada, teoria, formulario]
---

# Mapa y formulario general

Usa esta hoja para reconocer qué modelo físico conviene probar. La teoría y las justificaciones están separadas por tema.

## Cómo reconocer el tipo de ejercicio

| Si el enunciado pide… | Modelo que conviene probar primero |
|---|---|
| Campo o aceleración por varias masas | Calcula cada $GM/r^2$, descompón y suma vectores. |
| Peso a una altura o en superficie | Usa $r=R+h$ y la razón de cuadrados. |
| Rapidez, período o energía de una órbita circular | Empieza con equilibrio entre gravedad y fuerza centrípeta. |
| Rapidez de escape | Igualar energía total final a cero desde el radio inicial. |
| Radio orbital a partir de períodos, o masa central | Tercera ley de Kepler. |
| Tiempo o longitud entre observadores | Identifica el marco propio antes de usar $\gamma$. |
| Velocidad compuesta en relatividad | Define eje y signos; usa suma relativista. |
| Desplazamiento de aire desde presión | $k=2\pi f/v$ y $\Delta p_{max}=Bks_{max}$. |
| Nivel de varias fuentes | Suma intensidades lineales y luego calcula decibeles. |
| Frecuencia recibida por movimiento relativo | Fórmula Doppler con el medio como referencia. |
| Campos de una onda EM | $c=\lambda f$, $E_{max}=cB_{max}$ y regla de la mano derecha. |

## 1. Método general

1. Escribe datos, incógnita, sistema físico y unidades.
2. Dibuja la geometría, los vectores o los observadores.
3. Convierte a SI antes de sustituir: km a m, Mm a $10^6$ m, kN a $10^3$ N, nm a $10^{-9}$ m, años/días a segundos.
4. Escribe la relación física y despeja.
5. Sustituye con unidades; revisa dirección, signo y orden de magnitud.

Constantes frecuentes: $G=6.67\times10^{-11}\,\mathrm{N\,m^2/kg^2}$, $c=3.00\times10^8\,\mathrm{m/s}$, $g_0\approx9.81\,\mathrm{m/s^2}$. Usa las que indique el enunciado.

## Errores que cuestan puntos

- Usar altura $h$ en lugar de distancia al centro $R+h$.
- Sumar campos o velocidades sin revisar direcciones y signos.
- Usar el radio de superficie en una órbita a $5R$.
- Confundir peso con masa, tiempo propio con dilatado o longitud propia con contraída.
- Olvidar el cuadrado en las razones de gravedad y en el despeje de $v/c$.
- Convertir a decibeles antes de sumar intensidades.
- Confundir presión ambiente con amplitud de presión acústica.
- Omitir unidades, marco de referencia, dibujo o justificación de la fórmula.

## Teoría por tema

- [[Teoría/01 - Gravitación y órbitas]]
- [[Teoría/02 - Relatividad especial]] — [[Teoría/02 - Conceptos de relatividad especial|conceptos]] · [[Teoría/02 - Fórmulas aplicadas de relatividad especial|fórmulas]]
- [[Teoría/03 - Ondas y acústica]] — [[Teoría/03 - Conceptos de ondas y acústica|conceptos]] · [[Teoría/03 - Fórmulas aplicadas de ondas y acústica|fórmulas]]
- [[Teoría/04 - Ondas electromagnéticas]] — [[Teoría/04 - Conceptos de ondas electromagnéticas|conceptos]] · [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|fórmulas]]

## Autoevaluación integradora

Intenta responder cada pregunta sin abrir la explicación plegable. Después, compárala con el razonamiento y vuelve al módulo enlazado si algo no coincide.

**1. ¿Por qué no se puede sumar directamente el valor numérico de dos campos gravitatorios si apuntan en direcciones diferentes?**

> [!success]- Mostrar explicación
> El campo es un vector: cada masa produce una contribución dirigida hacia esa masa. Se suman por componentes, con sus signos; recién después se calcula el módulo y la dirección del resultado. Sumar solo los módulos pierde la información direccional. Repasa [[Teoría/01 - Conceptos de gravitación y órbitas#2. Varias fuentes: sumar flechas]].

**2. ¿Qué identifica al tiempo propio en relatividad y por qué no basta con elegir el intervalo más corto?**

> [!success]- Mostrar explicación
> El tiempo propio es el intervalo entre dos eventos que ocurren en el mismo lugar de un marco. Se identifica por la situación física y el marco que mide, no por comparar números después del cálculo. En otro marco esos eventos pueden ocurrir en lugares distintos y el intervalo medido es mayor: $\Delta t=\gamma\Delta t_0$. Repasa [[Teoría/02 - Conceptos de relatividad especial#4. Tiempo propio y dilatación temporal]].

**3. Dos fuentes sonoras independientes tienen la misma intensidad. ¿Se duplica el nivel en decibeles cuando ambas suenan?**

> [!success]- Mostrar explicación
> Se duplica la intensidad lineal, no el número de decibeles. Como el nivel usa un logaritmo, el aumento es $10\log_{10}(2)\approx3.01\,\mathrm{dB}$. Primero se suman intensidades y después se convierte el total. Repasa [[Teoría/03 - Conceptos de ondas y acústica#5. Decibeles: una escala logarítmica]].

**4. Si una onda electromagnética avanza hacia $+x$ y $\vec E$ apunta hacia $+y$, ¿cómo determinas $\vec B$ y la fase?**

> [!success]- Mostrar explicación
> El flujo de energía debe apuntar en el sentido de $\vec E\times\vec B$. Por tanto, $+\hat y\times\vec B=+\hat x$ exige $\vec B$ hacia $+\hat z$. Para avance en $+x$, una fase compatible es $kx-\omega t$. Comprueba el producto vectorial y el signo temporal por separado. Repasa [[Teoría/04 - Conceptos de ondas electromagnéticas#6. De una frase a los vectores]].

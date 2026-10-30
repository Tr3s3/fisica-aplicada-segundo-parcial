---
tags: [fisica-aplicada, teoria, conceptos, ondas-acustica]
---

# Conceptos — Ondas y acústica

**Volver al módulo:** [[Teoría/03 - Ondas y acústica]] · **Fórmulas y método:** [[Teoría/03 - Fórmulas aplicadas de ondas y acústica]] · **Práctica:** [[Ejercicios/03 - Ondas y acústica]]

## 1. Qué es lo que se propaga

Una onda es una perturbación que avanza y transporta energía. El medio puede oscilar alrededor de su posición de equilibrio sin viajar junto con la perturbación. En el sonido, por ejemplo, las moléculas de aire vibran localmente mientras las regiones de compresión y rarefacción avanzan hasta el oído.

Para una onda periódica:

- **Amplitud:** máxima variación respecto del equilibrio. En acústica puede ser desplazamiento de partícula $s_{\max}$ o presión $\Delta p_{\max}$; son amplitudes distintas.
- **Período $T$:** tiempo de una oscilación completa.
- **Frecuencia $f$:** ciclos por segundo; se mide en hertz, con $f=1/T$.
- **Longitud de onda $\lambda$:** distancia entre puntos consecutivos en la misma fase, por ejemplo dos compresiones.
- **Rapidez $v$:** avance de la fase de la onda por unidad de tiempo. No es, en general, la rapidez instantánea de las moléculas.

La onda sonora es **longitudinal**: las partículas del medio oscilan paralelas a la dirección de propagación. En una onda transversal, en cambio, oscilan perpendicularmente. Una curva sinusoidal que se dibuja para representar sonido suele mostrar presión o desplazamiento como función de la posición; no significa que el sonido viaje de arriba abajo.

![[imagenes/sonido-longitudinal.svg]]

## 2. El medio determina la rapidez del sonido

El sonido es una onda mecánica: necesita materia cuyas partes puedan comprimirse o deformarse y empujarse mutuamente. Por eso no se propaga en el vacío. Su rapidez depende de la elasticidad y la densidad del medio, no solo de la frecuencia.

En un fluido, una perturbación compresional tiene mayor rapidez cuando el medio es más rígido ante cambios de volumen y menor rapidez cuando es más denso. En un gas ideal, las compresiones y expansiones son aproximadamente adiabáticas durante una onda sonora; de ahí aparece la razón de calores específicos $\gamma$. En una varilla delgada se usa el módulo de Young $Y$. Las relaciones aplicables se resumen en [[Teoría/03 - Fórmulas aplicadas de ondas y acústica#2. Rapidez del sonido en cada medio]].

En problemas de examen a menudo se entrega la rapidez del sonido. En ese caso se usa el valor dado; no se vuelve a calcular desde la temperatura, densidad o elasticidad.

## 3. Compresión, presión y desplazamiento

Una partícula que se desplaza comprime el aire por delante y lo deja menos comprimido por detrás. La variación de presión $\Delta p$ describe cuánto sube o baja la presión local respecto del equilibrio. No es la presión atmosférica total.

Si una región de aire se comprime en una fracción pequeña, el módulo volumétrico $B$ conecta el cambio relativo de volumen con el cambio de presión. En una onda sinusoidal esa compresión depende de cuánto cambia el desplazamiento entre puntos vecinos; por eso interviene el número de onda $k=2\pi/\lambda$. El resultado para las amplitudes es $\Delta p_{\max}=Bks_{\max}$.

Presión y desplazamiento no alcanzan sus máximos en el mismo lugar y en el mismo instante: están desfasados un cuarto de ciclo. Cuando el desplazamiento local es máximo, la variación de presión allí pasa por cero; cuando hay compresión máxima, el desplazamiento local pasa por cero. La derivación y el uso para despejar $s_{\max}$ están en [[Teoría/03 - Fórmulas aplicadas de ondas y acústica#3. De presión a desplazamiento de las partículas]].

## 4. Intensidad: cuánta energía cruza una superficie

La **intensidad** $I$ es la potencia acústica media que atraviesa cada unidad de área perpendicular a la propagación. Se mide en $\mathrm{W/m^2}$. En una onda sinusoidal progresiva, transportar una amplitud de presión mayor requiere transportar más energía, y la intensidad es proporcional a $\Delta p_{\max}^2$.

La fórmula acústica en términos de presión supone una onda armónica que avanza en un medio uniforme. Si el dato es la presión eficaz (RMS) y no la amplitud máxima, la relación se escribe de otra forma; no mezcles ambas convenciones. En los problemas de este vault, $p_{\max}$ o $\Delta p_{\max}$ indica amplitud máxima.

Si una fuente puntual emite por igual en todas direcciones, la misma potencia se reparte sobre esferas cada vez mayores. Entonces la intensidad disminuye como $1/r^2$. Esta idea permite conectar potencia y distancia, aunque no sea uno de los planteos principales de los modelos.

## 5. Decibeles: una escala logarítmica

El oído puede percibir intensidades que cubren muchos órdenes de magnitud. El nivel sonoro $\beta$ expresa la razón entre la intensidad medida y una intensidad de referencia $I_0=10^{-12}\,\mathrm{W/m^2}$ mediante un logaritmo decimal.

Los decibeles no son una unidad lineal de intensidad. Por eso:

1. primero sumas las intensidades físicas de fuentes independientes;
2. después conviertes la intensidad total a decibeles.

Dos máquinas iguales e independientes aportan $I_{\mathrm{tot}}=2I$. El nivel sube $10\log_{10}(2)\approx3.01\,\mathrm{dB}$, no se duplica. Si las fuentes están sincronizadas y mantienen una diferencia de fase fija, la interferencia puede importar; la suma directa de intensidades corresponde al supuesto de fuentes independientes usado en el parcial.

## 6. Efecto Doppler: cambia la frecuencia recibida

El efecto Doppler es el cambio de frecuencia que registra un observador cuando cambia su movimiento relativo respecto de los frentes de onda. Para el sonido, el **medio** importa: el aire define la rapidez de propagación y las velocidades de fuente y observador se miden respecto de él.

### Si se mueve la fuente

Una fuente que avanza emite cada nuevo frente desde una posición adelantada respecto del anterior. En la dirección hacia la que se mueve, los frentes quedan más próximos: la longitud de onda disminuye. Como la rapidez del sonido en el aire sigue siendo la misma, la frecuencia de los frentes aumenta.

### Si se mueve el observador

Una fuente quieta deja frentes igualmente espaciados en el aire. Un observador que se mueve hacia la fuente encuentra más frentes por segundo; uno que se aleja encuentra menos. En este caso cambia la rapidez con que el observador intercepta los frentes, pero no la longitud de onda que ya está establecida en el aire.

### Si ambos se mueven

Se combinan los dos efectos: el movimiento de la fuente modifica el espaciamiento de los frentes y el del observador modifica cuántos de ellos intercepta por segundo. Antes de sustituir, dibuja el aire en reposo, la dirección de propagación y las dos velocidades. El esquema compara los casos:

![[imagenes/doppler-casos.svg]]

La convención y la derivación se desarrollan en [[Teoría/03 - Fórmulas aplicadas de ondas y acústica#6. Efecto Doppler: fórmula y signos]].

## 7. Cómo reconocer qué relación pide el enunciado

| Enunciado menciona… | Primero identifica… | Modelo de partida |
|---|---|---|
| Presión máxima y desplazamiento de partículas | Si la presión es una amplitud y qué rapidez/frecuencia tiene la onda | $k=2\pi f/v$ y $\Delta p_{\max}=Bks_{\max}$ |
| Intensidad y dB | Intensidad de referencia y si hay una o varias fuentes | $I=(\Delta p_{\max})^2/(2\rho v)$; luego $\beta$ |
| Dos o más fuentes | Si son independientes y qué intensidad aporta cada una | Suma de intensidades antes del logaritmo |
| Sirena, ambulancia o receptor móvil | Velocidades de fuente y receptor respecto del aire, y quién se acerca | Doppler; el movimiento de fuente y observador va en partes distintas |
| Frecuencia y longitud de onda | Rapidez de la onda en ese medio | $v=\lambda f$ |

## Secuencia antes de calcular

1. Dibuja el medio, la dirección de la onda y los objetos que se mueven.
2. Distingue amplitud de presión, presión ambiente e intensidad.
3. Convierte todos los datos a SI y anota si $p$ es amplitud máxima o eficaz.
4. Para varias fuentes, decide si corresponde sumar intensidades.
5. Para Doppler, define acercamiento o alejamiento respecto del aire antes de asignar signos.
6. Escribe primero la relación simbólica, despeja y recién después reemplaza números.
7. Comprueba el resultado: acercarse debe elevar la frecuencia y alejarse debe reducirla.

## Fuentes consultadas

- [Presentación de ondas y sonido](zotero://select/library/items/WFMW87CP): sonido y ondas longitudinales, PDF p. 12; rapidez en distintos medios, pp. 13–14; intensidad, p. 15; escala de decibeles, pp. 16–17; efecto Doppler y variables, pp. 18–19; ejemplos, pp. 20–22.
- [Práctica de sonido, Física Aplicada 2021](zotero://select/library/items/ZFCVVKE5): presión y desplazamiento, ejercicios 1–2; rapidez e intensidad, ejercicios 3–8; nivel sonoro y propagación, ejercicios 9–10; fuentes en fase, ejercicio 12; longitudes de onda y Doppler, ejercicios 13–17.
- Modelos cotejados: [segundo parcial 2023](zotero://select/library/items/YIXUYDMC), pregunta 2; [segundo parcial 2024](zotero://select/library/items/HQ9E54FP), pregunta 3; [segundo parcial 2025](zotero://select/library/items/DHM5X7QD), pregunta 1. La procedencia por ejercicio está en [[Fuentes Zotero y probabilidad#Ondas y acústica: fuentes consultadas para el módulo]].

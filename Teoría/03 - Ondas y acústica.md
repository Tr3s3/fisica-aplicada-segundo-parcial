---
tags: [fisica-aplicada, teoria, ondas-acustica]
---

# Ondas y acústica

**Recorrido:** [[Teoría/00 - Mapa y formulario general|Mapa general]] → [[Teoría/03 - Conceptos de ondas y acústica|Conceptos]] → [[Teoría/03 - Fórmulas aplicadas de ondas y acústica|Fórmulas]] → [[Ejercicios/03 - Ondas y acústica|Práctica]] → [[Resoluciones/03 - Ondas y acústica|Resoluciones]]

## Qué aparece en los modelos

En los modelos consultados se repiten tres familias:

1. **Presión y movimiento del aire:** obtener cuánto se desplazan las partículas a partir de la amplitud de presión.
2. **Intensidad y decibeles:** calcular el nivel de una fuente y el cambio al sumar dos fuentes iguales.
3. **Efecto Doppler:** distinguir una fuente que se mueve de un observador que se mueve, con el aire como referencia.

La práctica del TP amplía el alcance con familias que no aparecieron en los modelos revisados:

- rapidez del sonido en líquidos, gases y sólidos; longitud de onda y rango audible;
- propagación al oído y uso de ecos en sonar;
- potencia de una fuente, variación de intensidad con distancia y conversión entre intensidad y decibeles;
- interferencia de dos parlantes y reflexión en una pared;
- compresión de frentes delante y detrás de una fuente móvil y Doppler de eco.

La teoría distingue qué es central para el parcial y qué amplía la transferencia. Las relaciones, sus supuestos y el origen de cada fórmula están en las dos notas enlazadas arriba.

## Orden sugerido

1. Lee [[Teoría/03 - Conceptos de ondas y acústica]] para entender qué oscila, cómo se propaga el sonido y qué cambia en Doppler.
2. Usa [[Teoría/03 - Fórmulas aplicadas de ondas y acústica]] como hoja de selección, despeje y control de unidades.
3. Resuelve [[Ejercicios/03 - Ondas y acústica]] sin abrir las pistas ni la clave.
4. Reconstruye el planteo con [[Resoluciones/03 - Ondas y acústica]] y registra dónde elegiste un modelo distinto.

Para priorizar el tiempo, empieza por los ejercicios **M**. Luego practica los complementarios de prioridad media (**C20, C21, C23, C26 y C27**); deja para el repaso final los de prioridad baja (**C22, C24 y C25**).

## Esquemas del módulo

### Una onda mecánica longitudinal

![[imagenes/sonido-longitudinal.svg]]

### Efecto Doppler: separar el papel de la fuente y del observador

![[imagenes/doppler-casos.svg]]

Los esquemas de sonar e interferencia extraídos de la práctica están junto a la explicación en [[Teoría/03 - Conceptos de ondas y acústica#Frecuencia y longitud de onda al cambiar de medio]] y [[Teoría/03 - Conceptos de ondas y acústica#Superposición e interferencia]].

[[Teoría/03 - Conceptos de ondas y acústica#Fuentes consultadas|Fuentes y páginas consultadas]]

## Autoevaluación del módulo

Contesta sin mirar los apuntes y despliega cada explicación para revisar el razonamiento.

**1. ¿Qué tres familias de problemas acústicos aparecen en los modelos y qué decisión inicial exige cada una?**

> [!success]- Mostrar explicación
> Aparecen presión y desplazamiento del aire, intensidad y nivel sonoro, y efecto Doppler. Hay que distinguir amplitudes de presión y movimiento; decidir si se suman intensidades lineales antes de pasar a decibeles; y, para Doppler, identificar el movimiento de fuente y observador respecto del aire.

**2. ¿Por qué el movimiento de la fuente y el del observador aparecen de manera distinta en la fórmula Doppler del sonido?**

> [!success]- Mostrar explicación
> La fuente móvil modifica la separación entre frentes de onda en el aire y, por tanto, su longitud de onda. El observador móvil cambia cuántos frentes encuentra por segundo. El aire fija el marco de propagación, por eso las dos velocidades deben medirse respecto del medio.

**3. Dos fuentes iguales e independientes aumentan la intensidad total al doble. ¿Qué le ocurre al nivel sonoro?**

> [!success]- Mostrar explicación
> El nivel aumenta unos $3.01\,\mathrm{dB}$, no se duplica. La intensidad se suma linealmente y el nivel se calcula después con el logaritmo: $10\log_{10}(2I/I_0)=10\log_{10}(I/I_0)+10\log_{10}2$.

---
tags: [fisica-aplicada, teoria, ondas-em]
---

# Teoría — Ondas electromagnéticas

**Recorrido:** [[Teoría/00 - Mapa y formulario general|Mapa general]] → [[Teoría/04 - Conceptos de ondas electromagnéticas|conceptos]] → [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|fórmulas]] → [[Ejercicios/04 - Ondas electromagnéticas|práctica]] → [[Resoluciones/04 - Ondas electromagnéticas|resoluciones]]

> [!summary] Idea central
> Las leyes de Maxwell conectan los campos eléctrico y magnético variables y, en el vacío, producen una onda que avanza a $c$ sin medio material. En una onda plana sinusoidal, los campos oscilan en fase, son perpendiculares entre sí y al avance, y cumplen $E_{max}=cB_{max}$.

## Cómo estudiar este módulo

1. Lee [[Teoría/04 - Conceptos de ondas electromagnéticas|qué representa físicamente cada campo y cómo las leyes de Maxwell llevan a una onda]].
2. Estudia [[Teoría/04 - Fórmulas aplicadas de ondas electromagnéticas|de dónde salen las relaciones y cuándo usar cada fórmula]].
3. Resuelve primero el ejercicio 20, basado en el modelo; luego el 21, que invierte el sentido de avance y exige comprobar los signos.
4. Compara con las [[Resoluciones/04 - Ondas electromagnéticas|resoluciones paso a paso]] y vuelve a dibujar $\vec E$, $\vec B$ y la dirección de propagación.

## Esquemas

El primero muestra la orientación espacial de los campos. El segundo permite leer el sentido de viaje a partir del signo de la fase.

![[imagenes/onda-electromagnetica.svg]]

![[imagenes/sentido-fase-onda.svg]]

## Alcance para el parcial

Se practican ondas sinusoidales en el vacío: frecuencia, longitud de onda, amplitudes, número de onda, frecuencia angular, ecuaciones de campo y dirección de propagación. No se desarrolla óptica geométrica ni fenómenos de interfaz.

## Autoevaluación del módulo

Intenta explicar las decisiones sin consultar los formularios; abre luego la explicación plegable.

**1. En el vacío, si $\vec E$ apunta en $+y$ y la onda avanza en $+x$, ¿en qué sentido apunta $\vec B$?**

> [!success]- Mostrar explicación
> Debe cumplirse que $\vec E\times\vec B$ apunte en el sentido de propagación. Como $\hat y\times\hat z=\hat x$, el campo magnético apunta en $+z$. También puedes usar $\vec B=(1/c)\hat n\times\vec E$ y comprobar el resultado con $\vec E\times\vec B$.

**2. ¿Qué forma de fase describe una onda que viaja hacia $-x$ y cómo puedes comprobarlo?**

> [!success]- Mostrar explicación
> Una fase $kx+\omega t$ describe avance hacia $-x$. Mantén la fase constante y despeja la posición: $kx+\omega t=C$ implica $dx/dt=-\omega/k$. En cambio, $kx-\omega t$ da avance hacia $+x$.

**3. ¿Qué relación conecta las amplitudes de los campos en el vacío y por qué no significa que sean magnitudes con las mismas unidades?**

> [!success]- Mostrar explicación
> Se cumple $E_{max}=cB_{max}$. El factor $c$ convierte teslas, unidad de campo magnético, en voltios por metro, unidad de campo eléctrico. Sus valores numéricos no tienen que ser iguales y sus unidades siguen siendo diferentes.

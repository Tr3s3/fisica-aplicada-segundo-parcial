---
tags: [fisica-aplicada, resoluciones, ondas-acustica]
---

# Resoluciones modelo — Ondas y acústica

Lee cada resolución con lápiz y papel: pausa antes del despeje, predice el siguiente paso y justifica por qué aplica esa ley. Para practicar primero, usa [[Ejercicios/03 - Ondas y acústica]].

**Teoría relacionada:** [[Teoría/03 - Ondas y acústica]]

---

## Doppler de una ambulancia

![[imagenes/doppler-sonido.svg]]

Datos del modelo y la resolución: sirena $f=500\,\mathrm{Hz}$, rapidez del sonido $v_{snd}=340\,\mathrm{m/s}$.

### a) Fuente que se acerca a un observador quieto

Los frentes delante de la fuente quedan más juntos. $v_o=0$ y $v_s=+50\,\mathrm{m/s}$:
$$
f'=f\frac{v_{snd}}{v_{snd}-v_s}
=500\frac{340}{340-50}
=586.2\,\mathrm{Hz}.
$$

### b) Observador que se aleja de una fuente quieta

El observador encuentra menos frentes por segundo. $v_o=-30\,\mathrm{m/s}$ y $v_s=0$:
$$
f'=f\frac{v_{snd}+v_o}{v_{snd}}
=500\frac{340-30}{340}
=455.9\,\mathrm{Hz}.
$$
Chequeo: acercarse da una frecuencia mayor que $500\,\mathrm{Hz}$; alejarse, una menor.

## Desplazamiento del aire a partir de la amplitud de presión

![[imagenes/sonido-longitudinal.svg]]

Datos del DOCX 2025: $\Delta p_{max}=3.0\times10^{-2}\,\mathrm{Pa}$, $f=1000\,\mathrm{Hz}$, $v=344\,\mathrm{m/s}$, módulo volumétrico $B=1.42\times10^5\,\mathrm{Pa}$.

**1. Número de onda:** $k=2\pi f/v$:
$$
k=\frac{2\pi(1000)}{344}=18.27\,\mathrm{rad/m}.
$$

**2. Relación presión-desplazamiento:** para una onda sonora sinusoidal, $\Delta p_{max}=Bks_{max}$. Despeja:
$$
s_{max}=\frac{\Delta p_{max}}{Bk}
=\frac{3.0\times10^{-2}}{(1.42\times10^5)(18.27)}
=1.16\times10^{-8}\,\mathrm m.
$$
Resultado: $s_{max}\approx11.6\,\mathrm{nm}$. La presión atmosférica estándar del enunciado no se suma: la onda oscila alrededor de esa presión.

## Nivel sonoro de una y dos máquinas

La imagen del modelo 2023 parece indicar $I=2.0\times10^7\,\mathrm{W/m^2}$ por máquina. Se usa $I_0=10^{-12}\,\mathrm{W/m^2}$.

**1. Una máquina:**
$$
\beta_1=10\log_{10}\left(\frac{2.0\times10^7}{10^{-12}}\right)
=193.0\,\mathrm{dB}.
$$

**2. Dos máquinas independientes:** suma las intensidades, $I_{tot}=4.0\times10^7\,\mathrm{W/m^2}$:
$$
\beta_2=10\log_{10}\left(\frac{4.0\times10^7}{10^{-12}}\right)
=196.0\,\mathrm{dB}.
$$
La diferencia es $3.01\,\mathrm{dB}$. Si el exponente del original era $-7$, ambos niveles bajan $140\,\mathrm{dB}$ y la diferencia no cambia.

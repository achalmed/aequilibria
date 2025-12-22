---
documentmode: stu
course: Teoría y política monetaria
professor: Dr. Zenón Quispe Misaico
duedate: 05/11/2025
copyrightnotice: 2025
copyrightext: All rights reserved
title: Política monetaria del BCRP
subtitle: teoría y práctica
keywords:
- keyword1
- keyword2
categories:
- Macroeconomia
tags:
- macroeconomic
- politica_monetaria
author-note:
  status-changes:
    affiliation-change: null
    deceased: null
  disclosures:
    study-registration: null
    data-sharing: null
    related-report: null
    conflict-of-interest: El autor no tiene conflictos de interés que revelar.
    financial-support: null
    gratitude: null
    authorship-agreements: null
description: Análisis de los instrumentos y objetivos de política monetaria del Banco
  Central de Reserva del Perú, inflación objetivo y respuestas ante shocks externos.
eval: true
citation:
  type: article-journal
  author:
  - Edison Achalma
  pdf-url: https://aequilibria.netlify.app/posts/2025-05-11-teoria-y-politica-monetaria-bcrp/index.pdf
date: 05/11/2025
draft: false
jupyter: python3
image: ../featured.jpg
---

Dinero, eje central.

Bitcoin, activo altamente especulativo.

-   Transaccional
-   Inter temporal
-   óptimo
-   Dinámico, Ajuste de acuerdo a las necesidades
-   Estocástico (aleatorio)

::: {#be16d93a .cell}
``` {.python .cell-code}
import matplotlib.pyplot as plt
import numpy as np

# Configuración de la simulación
np.random.seed(42)  # Para reproducibilidad
n_days = 365  # Un año
base_happiness = 50  # Nivel base de felicidad
white_noise = np.random.normal(loc=0, scale=10, size=n_days)  # Ruido blanco: media 0, desv. estándar 10
happiness = base_happiness + white_noise  # Serie de felicidad
time = np.arange(n_days)

# Eventos estocásticos: uno positivo y uno negativo
event_positive_day = 100
event_negative_day = 250
happiness[event_positive_day] += 20  # Evento positivo
happiness[event_negative_day] -= 20  # Evento negativo

# Creación del gráfico
plt.figure(figsize=(10, 6))
plt.plot(time, happiness, label='Felicidad', color='blue', alpha=0.7)
plt.axhline(y=base_happiness, color='green', linestyle='--', label='Nivel base de felicidad')
plt.scatter([event_positive_day], [happiness[event_positive_day]], color='gold', s=100, label='Evento positivo')
plt.scatter([event_negative_day], [happiness[event_negative_day]], color='red', s=100, label='Evento negativo')
plt.title('Felicidad a través del tiempo')
plt.xlabel('Días')
plt.ylabel('Nivel de felicidad')
plt.grid(True)
plt.legend()

# Mostrar el gráfico
plt.show()

# Guardar el gráfico
#plt.savefig('happiness_over_time.png')
```
:::


Token Vale

-   Foward looking, decision hacia delante
-   Equilibrio general
-   Bienestar

Tenemos tres partes el bienestar menos el sacrificio del tiempo en la actividad - los usos i represntado por funcion de oscio (tiempo disponible), el resultado debe ser positivo

$$
L = Max E (\sum_{t = 1}^{\infty}  \beta_{t}  (u(C_{t}, \frac{M_{t}}{P_{t}},\epsilon_{t})) -  \int\limits_0^1 v(h_{t}(i),\epsilon_{t})di+) + \lambda (\int_{0}^{1} h_{t}(i) w_{t} (i)\,di + \int_{0}^{1} \pi_{t} (i) + \,di + M_{t-1} + \beta_{t-1}(1+R_{t-1}) )
$$

$$
- \int_{0}^{1} P_{t} (i) C_{t}\,di + M_{t} + \beta_{t} + T_{t}
$$

$\beta^{t}$ : Factor de actualización. Tiene un rendimiento $\frac{1}{1+R_{t}}$ debe ser iguak a renta de capital humano.

$u$ : Bienestar. Continu en el tiempo y espacio

$C_{t}$ Canasta de bienes y servicios. estatico (discreto) en el tiempo y espacio

$\frac{M_{t}}{P_{t}}$ : Valor real del dinero (líquido y divisible)

$\epsilon_{t}$ : Evento estocástico que afecta al bienestar

$h_{t}(i)$ :  Horas dedicadas a la actividad i

se agrega sumatoria por que tiene agreacion discreta

$w_{t}(i)$ : Salario que se paga por hacer i actividades

$\pi_{t} (i)$ : Renta que se paga por participar en actividad i

$M_{t}$ :  Dinero

$M_{t-1}$ : Dinero que tengo pero que decidí antes

$\beta_{t}$ : ahorro

$\beta_{t-1}(1+R_{t-1})$ :  ahorro capitalizado

$T_{t}$: impuesto

lo que mehos hecho es caracterizar el recurso disponible



# Publicaciones Similares

Si te interesó este artículo, te recomendamos que explores otros blogs y recursos relacionados que pueden ampliar tus conocimientos. Aquí te dejo algunas sugerencias:


1. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2021-07-19-01-conceptos-basicos/index.pdf) [01 Conceptos Basicos](https://aequilibria.netlify.app/posts/2021-07-19-01-conceptos-basicos)
2. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2021-07-26-02-teoria-de-consumo/index.pdf) [02 Teoria De Consumo](https://aequilibria.netlify.app/posts/2021-07-26-02-teoria-de-consumo)
3. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2021-08-02-03-teoria-de-la-inversion/index.pdf) [03 Teoria De La Inversion](https://aequilibria.netlify.app/posts/2021-08-02-03-teoria-de-la-inversion)
4. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2021-08-09-04-tipo-de-cambio/index.pdf) [04 Tipo De Cambio](https://aequilibria.netlify.app/posts/2021-08-09-04-tipo-de-cambio)
5. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2021-12-20-05-modelo-de-mundell-fleming/index.pdf) [05 Modelo De Mundell Fleming](https://aequilibria.netlify.app/posts/2021-12-20-05-modelo-de-mundell-fleming)
6. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2021-12-27-06-sector-externo/index.pdf) [06 Sector Externo](https://aequilibria.netlify.app/posts/2021-12-27-06-sector-externo)
7. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2022-01-03-07-fluctuaciones-de-corto-plazo/index.pdf) [07 Fluctuaciones De Corto Plazo](https://aequilibria.netlify.app/posts/2022-01-03-07-fluctuaciones-de-corto-plazo)
8. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2022-01-10-08-ciclos-economicos-reales-rbc/index.pdf) [08 Ciclos Economicos Reales Rbc](https://aequilibria.netlify.app/posts/2022-01-10-08-ciclos-economicos-reales-rbc)
9. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2022-01-17-09-crecimiento-economico/index.pdf) [09 Crecimiento Economico](https://aequilibria.netlify.app/posts/2022-01-17-09-crecimiento-economico)
10. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2022-01-24-10-economia-monetaria/index.pdf) [10 Economia Monetaria](https://aequilibria.netlify.app/posts/2022-01-24-10-economia-monetaria)
11. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2022-01-31-11-modelos-de-empleo/index.pdf) [11 Modelos De Empleo](https://aequilibria.netlify.app/posts/2022-01-31-11-modelos-de-empleo)
12. [{{< fa regular file-pdf >}}](https://aequilibria.netlify.app/posts/2025-05-11-teoria-y-politica-monetaria-bcrp/index.pdf) [Teoria Y Politica Monetaria Bcrp](https://aequilibria.netlify.app/posts/2025-05-11-teoria-y-politica-monetaria-bcrp)


Esperamos que encuentres estas publicaciones igualmente interesantes y útiles. ¡Disfruta de la lectura!


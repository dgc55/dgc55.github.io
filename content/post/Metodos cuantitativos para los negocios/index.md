---
author: Daniel Garcia
title: Métodos Cuantitativos para los Negocios
date: 2026-09-10
description: Esta es una breve explicación de los conceptos de cuantitativos de las ciencias de la administración, construyendo modelos y aplicaciones por computadora. Esto está aún en proceso así que haré actualizaciones continuas...
categories:
  - Maths
tags:
  - Industria
  - Algorithm
  - Optimice
image: cover.jpg
---
## Introducción 
Esta es una breve explicación de los conceptos de cuantitativos de las ciencias de la administración, construyendo
modelos y aplicaciones por computadora.

## Pronósticos y Análisis de Decisiones
## Programación Lineal y Optimización

### Introducción a la programación lineal
La programación lineal como tal nació por la necesitada de optimizar los recursos y logística en la segunda guerra mundial,
los aliados se encontraron con una escala logística sin precedentes: mover cantidades masivas de hombres al campo de batalla,
suministros y planificar ataques donde la superioridad del Eje era evidente. El padre de la PL, fue George Dantzig el cual
fue miembro del grupo SCOOP de la fuerza aérea de los EE.UU. y en 1947 publico el algoritmo Simplex, siendo hoy en dia
uno de los algoritmos más famosos, con el paso del tiempo estos conocimientos se fueron expandiendo al mundo empresarial donde encontró gran acojida
en la planificación de recursos, optimización de procesos y cadenas de suministro. Con el auge de la IA y la IA agentica
no ha desaparecido sino que lo ha vuelto más accesible para muchos, antes se tenia que tener un experto en formular un
modelo matemático ahora con el poder de razonamiento computacional se puede expresar con lenguaje natural.

### Problemas de programación lineal

Pondré algunos problemas usando lingo y traduciendo el codigo a pyomo una libreria de python,


Problema de distribución:
Una empresa tiene 3 plantas de producción y 4 centros de distribución. Necesita decidir cuántas unidades enviar de cada planta a cada centro para minimizar el costo total de transporte, satisfaciendo la oferta de cada planta y la demanda de cada centro.

Datos:

* Plantas (orígenes): P1, P2, P3

* Centros (destinos): C1, C2, C3, C4

*  Oferta (capacidad de producción): P1 = 100, P2 = 80, P3 = 120

*  Demanda (requerimiento): C1 = 70, C2 = 90, C3 = 80, C4 = 60

*  Costos unitarios de transporte ($Dolares/unidad$):

| Origen \ Destino | C1 | C2 | C3 | C4 |
| :--- | :---: | :---: | :---: | :---: |
| **P1** | 4 | 6 | 8 | 5 |
| **P2** | 7 | 5 | 3 | 6 |
| **P3** | 2 | 8 | 4 | 9 |



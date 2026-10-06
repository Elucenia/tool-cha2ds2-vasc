<!-- ELUCENIA technical documentation · cha2ds2-vasc · es · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/cha2ds2-vasc)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Insuficiencia cardíaca o disfunción ventricular izquierda

`icc`

### Hipertensión

`has`

### Edad

`idade`

- `0` — \< 65 años
- `1` — 65 a 74 años
- `2` — ≥ 75 años

### Diabetes

`dm`

### Ictus, AIT o tromboembolismo previo

`avc`

### Enfermedad vascular (infarto de miocardio previo, enfermedad arterial periférica, placa aórtica)

`vasc`

### Sexo femenino

`fem`

## Edición del método

CHA₂DS₂-VASc/Lip 2010 y CHA₂DS₂-VA/ESC 2024; máximo 9/8

## Fórmula documentada

C (insuficiencia cardíaca) 1 · H (hipertensión) 1 · A₂ (edad ≥ 75) 2 · D (diabetes) 1 · S₂ (ictus/AIT/TE) 2 · V (enfermedad vascular) 1 · A (65–74 años) 1 · Sc (sexo femenino) 1. Máximo: 9 puntos.

El CHA₂DS₂-VA (ESC 2024) es la misma puntuación sin el punto del sexo femenino.

## Límites y población

La publicación Lip 2010 evaluó la estratificación del tromboembolismo en pacientes con fibrilación auricular y describió una capacidad predictiva modesta de los esquemas comparados. Las categorías o tasas observadas en esa cohorte no garantizan un riesgo individual nulo. La variante CHA2DS2-VA y las decisiones de anticoagulación requieren la guía y la población correspondientes a la edición utilizada.

## Referencias

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

La información siguiente conserva las salidas del método para ejemplos sintéticos. No constituye una validación clínica independiente.

### 1

Anticoagulación oral recomendada (ESC 2024)

| Detalles del resultado | |
| --- | --- |
| CHA₂DS₂-VA (sin el sexo) | 8 puntos |
| ACV/TE por año sin anticoagulación | 15,2% |


### 2

Anticoagulación oral recomendada (ESC 2024)

| Detalles del resultado | |
| --- | --- |
| CHA₂DS₂-VA (sin el sexo) | 2 puntos |
| ACV/TE por año sin anticoagulación | 2,2% |


### 3

Sin indicación de anticoagulación por la puntuación (ESC 2024)

| Detalles del resultado | |
| --- | --- |
| CHA₂DS₂-VA (sin el sexo) | 0 puntos |
| ACV/TE por año sin anticoagulación | 1,3% |


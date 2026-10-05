<!-- ELUCENIA technical documentation · cha2ds2-vasc · en · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[conditions, sources and permissions](https://elucenia.org/en/tools/cha2ds2-vasc)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Heart failure or left ventricular dysfunction

`icc`

### Hypertension

`has`

### Age

`idade`

- `0` — \< 65 years
- `1` — 65 to 74 years
- `2` — ≥ 75 years

### Diabetes

`dm`

### Previous stroke, TIA or thromboembolism

`avc`

### Vascular disease (prior myocardial infarction, peripheral arterial disease, aortic plaque)

`vasc`

### Female sex

`fem`

## Method edition

CHA₂DS₂-VASc/Lip 2010 and CHA₂DS₂-VA/ESC 2024; maximum 9/8

## Documented formula

C (heart failure) 1 · H (hypertension) 1 · A₂ (age ≥ 75) 2 · D (diabetes) 1 · S₂ (stroke/TIA/TE) 2 · V (vascular disease) 1 · A (age 65–74) 1 · Sc (female sex) 1. Maximum: 9 points.

The CHA₂DS₂-VA (ESC 2024) is the same score without the female-sex point.

## Limits and population

Lip’s 2010 publication assessed thromboembolism stratification in patients with atrial fibrillation and described modest predictive ability for the compared schemes. Categories or rates observed in that cohort are not an individual guarantee of zero risk. The CHA2DS2-VA variant and anticoagulation decisions require the guideline and population corresponding to the edition used.

## References

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

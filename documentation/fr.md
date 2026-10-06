<!-- ELUCENIA technical documentation · cha2ds2-vasc · fr · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[conditions, sources et autorisations](https://elucenia.org/fr/outils/cha2ds2-vasc)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Insuffisance cardiaque ou dysfonction ventriculaire gauche

`icc`

### Hypertension

`has`

### Âge

`idade`

- `0` — \< 65 ans
- `1` — 65 à 74 ans
- `2` — ≥ 75 ans

### Diabète

`dm`

### AVC, AIT ou événement thromboembolique antérieur

`avc`

### Maladie vasculaire (infarctus du myocarde antérieur, artériopathie périphérique, plaque aortique)

`vasc`

### Sexe féminin

`fem`

## Édition de la méthode

CHA₂DS₂-VASc/Lip 2010 et CHA₂DS₂-VA/ESC 2024 ; maximum 9/8

## Formule documentée

C (insuffisance cardiaque) 1 · H (hypertension) 1 · A₂ (âge ≥ 75) 2 · D (diabète) 1 · S₂ (AVC/AIT/TE) 2 · V (maladie vasculaire) 1 · A (65–74 ans) 1 · Sc (sexe féminin) 1. Maximum : 9 points.

Le CHA₂DS₂-VA (ESC 2024) est le même score sans le point du sexe féminin.

## Limites et population

La publication Lip 2010 a évalué la stratification du risque thromboembolique chez des patients atteints de fibrillation atriale et a décrit une capacité prédictive modeste des systèmes comparés. Les catégories ou taux observés dans cette cohorte ne garantissent pas individuellement un risque nul. La variante CHA2DS2-VA et les décisions d’anticoagulation exigent les recommandations et la population correspondant à l’édition utilisée.

## Références

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Anticoagulation orale recommandée (ESC 2024)

| Détails du résultat | |
| --- | --- |
| CHA₂DS₂-VA (sans le sexe) | 8 points |
| AVC/TE par an sans anticoagulation | 15,2% |


### 2

Anticoagulation orale recommandée (ESC 2024)

| Détails du résultat | |
| --- | --- |
| CHA₂DS₂-VA (sans le sexe) | 2 points |
| AVC/TE par an sans anticoagulation | 2,2% |


### 3

Aucune indication d’anticoagulation selon le score (ESC 2024)

| Détails du résultat | |
| --- | --- |
| CHA₂DS₂-VA (sans le sexe) | 0 points |
| AVC/TE par an sans anticoagulation | 1,3% |


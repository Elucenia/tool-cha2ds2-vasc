<!-- ELUCENIA technical documentation · cha2ds2-vasc · it · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/cha2ds2-vasc)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Insufficienza cardiaca o disfunzione ventricolare sinistra

`icc`

### Ipertensione

`has`

### Età

`idade`

- `0` — \< 65 anni
- `1` — 65 a 74 anni
- `2` — ≥ 75 anni

### Diabete

`dm`

### Ictus, TIA o tromboembolia pregressi

`avc`

### Malattia vascolare (pregresso infarto miocardico, arteriopatia periferica, placca aortica)

`vasc`

### Sesso femminile

`fem`

## Edizione del metodo

CHA₂DS₂-VASc/Lip 2010 e CHA₂DS₂-VA/ESC 2024; massimo 9/8

## Formula documentata

C (scompenso cardiaco) 1 · H (ipertensione) 1 · A₂ (età ≥ 75) 2 · D (diabete) 1 · S₂ (ictus/TIA/TE) 2 · V (malattia vascolare) 1 · A (65–74 anni) 1 · Sc (sesso femminile) 1. Massimo: 9 punti.

Il CHA₂DS₂-VA (ESC 2024) è lo stesso punteggio senza il punto del sesso femminile.

## Limiti e popolazione

La pubblicazione Lip 2010 ha valutato la stratificazione del tromboembolismo in pazienti con fibrillazione atriale e ha descritto una capacità predittiva modesta degli schemi confrontati. Le categorie o i tassi osservati in quella coorte non garantiscono un rischio individuale nullo. La variante CHA2DS2-VA e le decisioni sull’anticoagulazione richiedono la linea guida e la popolazione corrispondenti all’edizione utilizzata.

## Riferimenti

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Anticoagulazione orale raccomandata (ESC 2024)

| Dettagli del risultato | |
| --- | --- |
| CHA₂DS₂-VA (senza il sesso) | 8 punti |
| ICTUS/TE all’anno senza anticoagulazione | 15,2% |


### 2

Anticoagulazione orale raccomandata (ESC 2024)

| Dettagli del risultato | |
| --- | --- |
| CHA₂DS₂-VA (senza il sesso) | 2 punti |
| ICTUS/TE all’anno senza anticoagulazione | 2,2% |


### 3

Nessuna indicazione all’anticoagulazione in base al punteggio (ESC 2024)

| Dettagli del risultato | |
| --- | --- |
| CHA₂DS₂-VA (senza il sesso) | 0 punti |
| ICTUS/TE all’anno senza anticoagulazione | 1,3% |


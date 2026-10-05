<!-- ELUCENIA technical documentation · cha2ds2-vasc · de · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/cha2ds2-vasc)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Herzinsuffizienz oder linksventrikuläre Dysfunktion

`icc`

### Hypertonie

`has`

### Alter

`idade`

- `0` — \< 65 Jahre
- `1` — 65 bis 74 Jahre
- `2` — ≥ 75 Jahre

### Diabetes

`dm`

### Früherer Schlaganfall, TIA oder Thromboembolie

`avc`

### Gefäßerkrankung (früherer Myokardinfarkt, periphere arterielle Erkrankung, Aortenplaque)

`vasc`

### Weibliches Geschlecht

`fem`

## Fassung der Methode

CHA₂DS₂-VASc/Lip 2010 und CHA₂DS₂-VA/ESC 2024; Maximum 9/8

## Dokumentierte Formel

C (Herzinsuffizienz) 1 · H (Hypertonie) 1 · A₂ (Alter ≥ 75) 2 · D (Diabetes) 1 · S₂ (Schlaganfall/TIA/TE) 2 · V (Gefäßerkrankung) 1 · A (65–74 Jahre) 1 · Sc (weibliches Geschlecht) 1. Maximum: 9 Punkte.

Der CHA₂DS₂-VA (ESC 2024) ist derselbe Score ohne den Punkt für weibliches Geschlecht.

## Grenzen und Population

Lip 2010 untersuchte die Thromboembolierisikostratifizierung bei Patienten mit Vorhofflimmern und beschrieb eine mäßige Vorhersageleistung der verglichenen Systeme. Kategorien oder beobachtete Raten dieser Kohorte garantieren individuell kein Nullrisiko. Die Variante CHA2DS2-VA und Entscheidungen zur Antikoagulation erfordern die zur verwendeten Ausgabe passende Leitlinie und Population.

## Referenzen

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

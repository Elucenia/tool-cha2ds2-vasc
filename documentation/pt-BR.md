<!-- ELUCENIA technical documentation · cha2ds2-vasc · pt-BR · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/cha2ds2-vasc)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Insuficiência cardíaca ou disfunção de VE

`icc`

### Hipertensão

`has`

### Idade

`idade`

- `0` — \< 65 anos
- `1` — 65 a 74 anos
- `2` — ≥ 75 anos

### Diabetes

`dm`

### AVC, AIT ou tromboembolismo prévio

`avc`

### Doença vascular (IAM prévio, doença arterial periférica, placa aórtica)

`vasc`

### Sexo feminino

`fem`

## Edição do método

CHA 2 DS 2 VASc/Lip 2010 e CHA 2 DS 2 VA/ESC 2024; máximo 9/8

## Fórmula documentada

C (ICC) 1 · H (hipertensão) 1 · A₂ (idade ≥ 75) 2 · D (diabetes) 1 · S₂ (AVC/AIT/TE) 2 · V (doença vascular) 1 · A (65 a 74 anos) 1 · Sc (sexo feminino) 1. Máximo: 9 pontos.

O CHA₂DS₂-VA (ESC 2024) é o mesmo escore sem o ponto do sexo feminino.

## Limites e população

A publicação Lip 2010 avaliou estratificação de tromboembolismo em pacientes com fibrilação atrial e descreveu capacidade preditiva modesta dos esquemas comparados. Categorias ou taxas observadas nessa coorte não são uma garantia individual de risco zero. A variante CHA2DS2-VA e decisões de anticoagulação exigem a diretriz e a população correspondentes à edição utilizada.

## Referências

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

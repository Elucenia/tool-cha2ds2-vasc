<!-- ELUCENIA technical documentation · cha2ds2-vasc · ja · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[条件・出典・許諾](https://elucenia.org/ja/tools/cha2ds2-vasc)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 心不全または左室機能障害

`icc`

### 高血圧

`has`

### 年齢

`idade`

- `0` — \< 65 歳
- `1` — 65 ～ 74 歳
- `2` — ≥ 75 歳

### 糖尿病

`dm`

### 脳卒中、TIA、血栓塞栓症の既往

`avc`

### 血管疾患（心筋梗塞の既往、末梢動脈疾患、大動脈プラーク）

`vasc`

### 女性

`fem`

## 方法の版

CHA₂DS₂-VASc/Lip 2010とCHA₂DS₂-VA/ESC 2024；最高9/8

## 記載された計算式

C（心不全） 1 · H（高血圧） 1 · A₂ (年齢 ≥ 75) 2 · D（糖尿病） 1 · S₂（脳卒中/TIA/血栓塞栓症） 2 · V（血管疾患） 1 · A (65～74歳) 1 · Sc（女性） 1. 最高9点。

このCHA₂DS₂-VA (ESC 2024) は女性の1点を除いた同じスコアです。

## 限界・対象集団

Lip 2010の論文は、心房細動患者の血栓塞栓症の層別化を評価し、比較した方式の予測能力は限定的であると記載しました。そのコホートで観察された区分や発生率は、個人のリスクがゼロであることを保証しません。CHA2DS2-VAの変法や抗凝固の判断には、使用する版に対応したガイドラインと対象集団が必要です。

## 参考文献

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

経口抗凝固療法が推奨される（ESC 2024）

| 結果の詳細 | |
| --- | --- |
| CHA₂DS₂-VA（性別なし） | 8 点 |
| 抗凝固療法なしの年間脳卒中/TE | 15.2% |


### 2

経口抗凝固療法が推奨される（ESC 2024）

| 結果の詳細 | |
| --- | --- |
| CHA₂DS₂-VA（性別なし） | 2 点 |
| 抗凝固療法なしの年間脳卒中/TE | 2.2% |


### 3

スコアによる抗凝固療法の適応なし（ESC 2024）

| 結果の詳細 | |
| --- | --- |
| CHA₂DS₂-VA（性別なし） | 0 点 |
| 抗凝固療法なしの年間脳卒中/TE | 1.3% |


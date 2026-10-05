<!-- ELUCENIA technical documentation · cha2ds2-vasc · zh · no clinical/professional/rights approval -->

# CHA₂DS₂-VASc

[条件、来源与许可](https://elucenia.org/zh/tools/cha2ds2-vasc)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 心力衰竭或左心室功能障碍

`icc`

### 高血压

`has`

### 年龄

`idade`

- `0` — \< 65 岁
- `1` — 65 至 74 岁
- `2` — ≥ 75 岁

### 糖尿病

`dm`

### 既往卒中、短暂性脑缺血发作或血栓栓塞

`avc`

### 血管疾病（既往心肌梗死、外周动脉疾病、主动脉斑块）

`vasc`

### 女性

`fem`

## 方法版本

CHA₂DS₂-VASc/Lip 2010与CHA₂DS₂-VA/ESC 2024；最高9/8

## 已记录的公式

C（心力衰竭） 1 · H（高血压） 1 · A₂ (年龄 ≥ 75) 2 · D（糖尿病） 1 · S₂（卒中/TIA/血栓栓塞） 2 · V（血管疾病） 1 · A (65–74岁) 1 · Sc（女性） 1. 最高9分。

该CHA₂DS₂-VA (ESC 2024) 与原评分相同，但不计女性分。

## 限制与适用人群

Lip 2010论文评估了心房颤动患者的血栓栓塞分层，并指出所比较方案的预测能力有限。该队列观察到的类别或发生率，不能保证某个个体风险为零。CHA2DS2-VA变体和抗凝决策，需要所用版本对应的指南及人群。

## 参考文献

- [Lip GYH et al. Refining clinical risk stratification for predicting stroke and thromboembolism in atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.09-1584)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

- [Hindricks G et al. 2020 ESC Guidelines for the diagnosis and management of atrial fibrillation. Eur Heart J, 2021.](https://doi.org/10.1093/eurheartj/ehaa612)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

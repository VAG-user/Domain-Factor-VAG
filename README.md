# Domain-Factor Value-Action Gap Dataset

## English version

This directory organizes the Japanese-language topics, few-shot examples for LLM-based generation, the completed dataset of action scenarios used in this study, and the prompts provided to LLMs. It is intended to be maintained as an independent data repository.

## Structure

```text
domain-factor-VAG/
├── _full-dataset/  # Completed full dataset of action scenarios by domain and factor, used in this study
├── few-shots/      # Examples referenced when generating action scenarios
├── prompts/        # Prompts provided as input to LLMs
├── topics/         # Domains, subcategories, and topics
└── README.md
```

The domains covered are environmentally responsible behavior, prosocial behavior, and health behavior.

## Directories

### `_full-dataset`

The completed dataset of action scenarios organized by domain, factor, and topic. Each record contrasts which value is prioritized: a value associated with the domain or one associated with an external factor.

### `few-shots`

Examples used as references when LLMs generate action scenarios. Each example includes topic information and two scenarios that contrast which value is prioritized.

### `prompts`

Prompts used as inputs to LLMs in this study. The directory contains three types: data generation, Task 1 for choosing which value to prioritize, and Task 2 for choosing an action scenario. Placeholders such as `{country}` and `{topic}` are replaced with values from the relevant data during the experiments.

### `topics`

Topics and subcategories for each domain. Each topic is identified by a `topic_id` and referenced by the other data files.

---

## 日本語 (Japanese original version)

本ディレクトリは、本研究で使用した日本語版のトピック、LLM生成用のfew-shots具体例、作成した完成版のデータセット(行動シナリオ)、入力用プロンプトを、独立したデータリポジトリとして整理しています。

## 構成

```text
domain-factor-VAG/
├── _full-dataset/      # 領域×要因ごとの行動シナリオデータ (本研究の実験で使用した、完成版のフルデータセット)
├── few-shots/    # 行動シナリオ生成時に参照する具体例
├── prompts/      # LLM入力用プロンプト
├── topics/       # 領域・サブカテゴリ・トピックの一覧
└── README.md
```

対象領域は、環境配慮行動、向社会的行動、健康行動です。

## 各ディレクトリ

### `_full-dataset`

各領域・要因・トピックに対応する行動シナリオの、完成版のデータセットです。各レコードは、領域に関する価値観と外的要因に関する価値観の優先順位が対照的になるように構成されています。

### `few-shots`

LLMによる行動シナリオ生成の参考例です。各例にはトピック情報と、価値観の優先順位が対照的な2つの行動シナリオが含まれます。

### `prompts`

本研究で使用したLLM入力用プロンプトを収録しています。データ生成、価値観の優先順位を選択するTask 1、行動シナリオを選択するTask 2の3種類を含みます。本文中の `{country}` や `{topic}` などのプレースホルダーには、実験時に対象データの値を代入します。

### `topics`

各領域のトピックとサブカテゴリを収録しています。トピックは `topic_id` で識別され、他のデータから参照されます。

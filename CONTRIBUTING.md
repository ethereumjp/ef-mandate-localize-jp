# ef-mandate-localize-jp へのコントリビュート

このリポジトリは、Ethereum Foundation Mandate を日本語化するためのものです。翻訳の修正、補足、解釈、質問、論点整理などの形で貢献できます。

## プロジェクトの目的

このプロジェクトは、単一の「公式」かつ完全に忠実な日本語訳を作ることを目的としていません。

目的は次のとおりです。

- 日本語読者が Mandate を理解しやすくする
- 有用な文脈や複数の読みを残す
- 質問や異論を公開の場で扱えるようにする
- 周辺の文脈変化にあわせて翻訳を継続的に更新する

つまり、このローカライズは一度完成して終わる作業ではなく、継続的に更新されるものとして扱います。

## ソースの扱い

- 原文の英語は `source/en/chapters/` に置きます。
- 日本語訳は `source/ja/chapters/` に置きます。
- 英語版と日本語版の章番号は対応させます。
- `01-`、`02-`、`03-` のような番号付きプレフィックスで章順を保ちます。
- 生成物である `dist/` は編集しません。

## リポジトリ構成

- 1 章につき 1 Markdown ファイルを基本とします。
- 繰り返し出る用語や名称は `GLOSSARY.md` を参照します。
- 用語は章をまたいで統一します。
- 1 章、または密接に関連する少数の章に絞った小さめの PR を優先します。
- 公開用ではないメモは、本文ではなくコメントや別の作業メモに残します。

## Contribution Types

以下のいずれかとしてラベル付けしてください。

- `Question`: なぜこの表現なのか、何を指すのかを問うもの
- `Commentary`: 解釈、文脈補足、論点整理
- `Critique`: 異論、懸念、違和感の表明
- `Localization note`: 日本コミュニティの文脈での意味づけ
- `Clarification`: 用語や背景の説明

## 基本原則

### 直訳を目的にしない

英語の語順や構文をそのまま残すことより、自然な日本語として読めることを優先します。ただし、原意は保ちます。

### 公式 EF 翻訳として扱わない

このプロジェクトは、EF の意図を推測して代弁する場ではありません。参加者がどう読んだかを基準にします。

### 原文への敬意を保つ

原文の主張を歪めないでください。補足や解釈は歓迎しますが、原文に根拠のある形にとどめます。

### ローカル文脈は含めてよい

日本の Ethereum コミュニティから見た含意、違和感、期待、論点は明示して構いません。

## 書き方のルール

- 1 つの contribution は 1 つの論点に絞ります。
- 可能であれば、原文の該当箇所を明示します。
- 事実説明と意見は分けます。
- 解釈を含む場合は、上記の contribution type を明示します。
- 「EF はこう言いたいはず」のような断定は避けます。
- 「私はこう読んだ」「私たちはこう読んだ」のように主語を明確にします。
- 複数の読みがある場合は、1 つに統合せず並記します。

## GitHub 上の運用

GitHub Issue と Pull Request は次のように使い分けます。

- `Issue`: 質問、論点提起、未解決の解釈上の問題
- `Pull request`: 文面の変更提案

Issue や PR には、できれば次を含めてください。

- 対象箇所
- contribution type
- 内容
- 必要であれば理由

不明瞭な箇所や意見が割れる箇所では、次のように扱います。

- 必要なら複数の読みを並記する
- `Reading A` / `Reading B` や `Interpretation A` / `Interpretation B` のような見出しを使う
- 長い補足は `<details>` を使って折りたたむ

## レビューチェック

- 章番号が正しく揃っている
- 見出しレベルが一貫している
- 用語が一貫している
- Markdown がきれいにレンダリングされる
- 英語版と日本語版の章番号が揃っている
- 生成済みの本文と PDF がビルドできる

## Code of Conduct

このリポジトリの行動規範は [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) を参照してください。

---

# Contributing to ef-mandate-localize-jp

This repository localizes the Ethereum Foundation Mandate into Japanese. Contributions are welcome in the form of translation edits, clarifications, commentary, questions, and discussion notes.

## Project Goal

The goal of this project is not to produce a single "official" or perfectly faithful Japanese translation.

Instead, the project aims to:

- help Japanese readers understand the Mandate,
- preserve useful context and alternative readings,
- surface questions and disagreements openly, and
- keep the translation evolving as the surrounding context changes.

In other words, localization here is treated as an ongoing process rather than a one-time completion step.

## Source Of Truth

- Keep the original English text in `source/en/chapters/`.
- Keep the Japanese translation in `source/ja/chapters/`.
- Keep chapter numbers aligned between English and Japanese.
- Keep chapter order stable with numeric prefixes such as `01-`, `02-`, `03-`.
- Do not edit generated files in `dist/`.

## Repository Structure

- One chapter per Markdown file.
- Use `GLOSSARY.md` for recurring terms and names.
- Keep terminology consistent across chapters.
- Prefer small pull requests that cover one chapter or a tightly related set of chapters.
- If you need to leave a note that is not ready for publication, put it in a comment or separate working note rather than in the final manuscript.

## Contribution Types

Contributions should be labeled as at least one of the following:

- `Question`: asks why a phrase was chosen or what a passage means.
- `Commentary`: adds interpretation, context, or discussion.
- `Critique`: states disagreement, concern, or a point of tension.
- `Localization note`: explains local meaning or implications for the Japanese community.
- `Clarification`: defines a term or explains background.

## Core Principles

### Do not aim for a literal translation

The project is not trying to preserve English sentence structure at the expense of readability. Natural Japanese is preferred when it still preserves the original intent.

### Do not present the result as an official EF translation

Contributions should reflect how participants read the text, not what they assume the EF "must have meant."

### Respect the original text

Do not distort the original argument. Additions are welcome when they help readers understand the text better, but they should remain grounded in the source.

### Local context is allowed

It is acceptable to surface implications, discomfort, expectations, and discussion points from the perspective of the Japanese Ethereum community.

## Writing Rules

- One contribution should focus on one point.
- Where possible, identify the relevant passage in the source text.
- Separate factual explanation from opinion.
- Label interpretive content clearly with one of the contribution types above.
- Avoid statements like "the EF must mean this."
- Prefer phrasing such as "I read this as..." or "we read this as..."
- If multiple interpretations exist, keep them side by side instead of forcing one into the final wording.

## GitHub Workflow

Use GitHub issues and pull requests for different kinds of work:

- `Issue`: questions, discussion points, and open interpretive questions.
- `Pull request`: proposed text changes.

When opening an issue or PR, include:

- the target passage,
- the contribution type,
- the content itself,
- and a reason if the point is not self-evident.

For disagreements or ambiguous passages:

- keep multiple readings visible when useful,
- use headings such as `Reading A` / `Reading B` or `Interpretation A` / `Interpretation B`,
- and use `<details>` blocks for longer side notes when appropriate.

## Review Checklist

- Chapter numbering is correct and complete.
- Heading levels are consistent.
- Glossary terms are used consistently.
- Markdown renders cleanly.
- English and Japanese chapter numbers stay in sync.
- The merged manuscript and PDF build successfully.

## Code Of Conduct

Please read and follow the repository's [Code of Conduct](CODE_OF_CONDUCT.md).

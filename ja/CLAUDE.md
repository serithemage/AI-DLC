# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

本リポジトリは、AWS Raja SPの **AI-DLC (AI-Driven Development Lifecycle)** 方法論を日本語に翻訳した文書である。これはソフトウェア開発プロジェクトではなく、**文書専用リポジトリ** である。

- **原著者:** Raja SP (Amazon Web Services)
- **目的:** AIネイティブソフトウェア開発方法論に関する日本語教育資料の提供
- **ホスティング:** GitHub Pages (https://serithemage.github.io/AI-DLC/)
- **著作権:** すべての権利は原著者に帰属する

## Documentation Structure

```
AI-DLC/
├── AI-Driven Development Liftcycle.md    # 韓国語主文書 (2,837+ 行)
├── index.md                               # GitHub Pages 韓国語版
├── README.md                              # リポジトリ概要 (韓国語)
├── CLAUDE.md                              # Claude Code作業ガイド (韓国語)
├── _config.yml                            # Jekyll設定 (theme: cayman)
├── ja/                                    # 日本語版ディレクトリ
│   ├── index.md                           # GitHub Pages 日本語版
│   ├── README.md                          # リポジトリ概要 (日本語)
│   └── CLAUDE.md                          # Claude Code作業ガイド (日本語)
└── images/                                # ダイアグラム (共有)
    ├── ai-dlc-framework.png
    ├── ai-dlc-workflow.png
    └── ai-dlc-detailed-workflow.png
```

**重要:** 日本語文書を更新する際は、`ja/`ディレクトリ内のファイルを修正する。画像は`../images/`パスで参照する。

## Translation Standards

### 英文維持用語 (Technical Terms)
次の用語は英語で維持:
- **Core Concepts:** Intent, Unit, Bolt, Domain Design, Logical Design, Deployment Unit
- **Design Techniques:** DDD (Domain-Driven Design), BDD (Behavior-Driven Design), TDD (Test-Driven Development)
- **Ceremonies:** Mob Elaboration, Mob Construction
- **Technologies:** CI/CD, DevOps, GenAI, LLM, API, AWS, Lambda, DynamoDB, Kubernetes, Terraform

### 日本語翻訳用語
| English | 韓国語 | 日本語 |
|---------|---------|---------|
| Intent | 의도 | インテント (意図) |
| Unit | 유닛 | ユニット |
| Bolt | 볼트 | ボルト |
| Inception | 인셉션 | インセプション |
| Construction | 구성 | 構築 |
| Operations | 운영 | 運用 |
| Greenfield | 그린필드 | グリーンフィールド |
| Brownfield | 브라운필드 | ブラウンフィールド |
| Mob Elaboration | 몹 엘라보레이션 | モブエラボレーション |
| Mob Construction | 몹 구성 | モブ構築 |
| Domain Design | 도메인 설계 | ドメイン設計 |
| Logical Design | 논리 설계 | 論理設計 |

### 翻訳原則
- 技術用語は英文維持、説明は日本語に翻訳
- 原文のMarkdown構造を維持 (見出し、テーブル、コードブロック)
- ダイアグラム参照パスを正確に維持
- **である体を使用** (技術文書スタイル)

## である体 Style Guidelines

本プロジェクトの日本語翻訳は **である体** (平叙体)を使用する。これは技術文書に適した簡潔で客観的な文体である。

### である体パターン規則

| です・ます体 | である体 |
|------------|----------|
| だ | である |
| です | である |
| します | する |
| されます | される |
| できます | できる |
| ありません | ない |

### である体使用例

❌ **誤り** (です・ます体):
```
AI-DLCは開発プロセスを最適化します。
これは重要な概念です。
AIが計画を生成します。
```

✅ **正しい** (である体):
```
AI-DLCは開発プロセスを最適化する。
これは重要な概念である。
AIが計画を生成する。
```

### である体一貫性チェックリスト
- すべての平叙文はである/する/できるで終わる
- 技術定義はである体を使用: "ユニットとは...である"
- プロセス説明はである体を使用: "AIが分析する"
- 質問にはかを使用可能: "適切であるか"

## Key AI-DLC Concepts

AI-DLC方法論の核心概念理解のための参考:

### 3段階フレームワーク
1. **Inception (インセプション):** Intentキャプチャ → Unitへの分解 (Mob Elaborationを通じて)
2. **Construction (構築):** Domain Design → Logical Design → コード生成 (Mob Constructionを通じて)
3. **Operations (運用):** デプロイ、モニタリング、メンテナンス

### コア成果物
- **Intent:** 高レベルビジネス目標
- **Unit:** 凝集性のある作業要素
- **Bolt:** 迅速な反復サイクル (時間/日単位)
- **Domain Design:** DDDを活用したビジネスロジックモデリング
- **Logical Design:** アーキテクチャパターンを通じたNFR適用

### 10のコア原則
文書で詳細に説明されるAI-DLCの基礎哲学 (再構想、対話方向逆転、コア設計技法統合など)

## GitHub Pages Workflow

### 自動デプロイ
- `main`ブランチにプッシュするとGitHubが自動的にPagesをビルド/デプロイ
- Jekyllが`_config.yml`設定に従って静的サイトを生成
- **手動ビルドコマンド不要** (GitHub Actionsが自動処理)

### ローカルプレビュー (オプション)
```bash
bundle install
bundle exec jekyll serve
# http://localhost:4000 で確認
```

### 言語切り替え
- 韓国語版: https://serithemage.github.io/AI-DLC/
- 日本語版: https://serithemage.github.io/AI-DLC/ja/

## Content Management Guidelines

### 文書更新時
1. 韓国語版を更新する場合: `index.md`を修正
2. 日本語版を更新する場合: `ja/index.md`を修正
3. 両バージョンの内容を同期させる必要がある場合は両方を更新
4. ダイアグラム追加/変更時は`images/`ディレクトリに保存
5. Markdown画像参照パス:
   - 韓国語版: `![説明](images/ファイル名.png)`
   - 日本語版: `![説明](../images/ファイル名.png)`

### コミットメッセージ
- 日本語または英語使用可能
- Co-authored-byタグ含めることを推奨

### 著作権表記
原著者帰属表記を維持:
- README-ja.md下部の著作権文言を保存
- 原文リンクを維持

## Important Notes

- **ビルド/テスト/Lintコマンドなし:** 本リポジトリは文書専用のため、`package.json`、テストフレームワーク、Linter設定が存在しない
- **依存関係インストール不要:** 純粋Markdown + Jekyll (GitHubで自動処理)
- **コード実行なし:** 実行可能なコードは含まれていない
- **翻訳正確性優先:** AI-DLC方法論の意図を正確に伝達することがコア目標
- **である体一貫性:** 日本語翻訳文書では必ずである体を使用すること

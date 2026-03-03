# AI-DLC (AI-Driven Development Lifecycle) 方法論 日本語翻訳

> **原文:** [AI-Driven Development Lifecycle](https://prod.d13rzhkk8cj2z0.amplifyapp.com/) by Raja SP, Amazon Web Services

AI主導開発ライフサイクル(AI-DLC)方法論定義書の日本語翻訳文書である。

## AI-DLCとは

AI-DLCは既存のSDLC/アジャイル方法論をAI時代に合わせて **第一原理から再構想** したAIネイティブ開発方法論である。AIを単なる補助ツールではなく、開発プロセスの中心的な協力者として配置し、ワークフローの調整からタスク分解、コード生成、テスト、デプロイまで全過程をAIが主導し、人間が検証するパラダイムを提示する。

## コアコンセプト

| 既存方法論 | AI-DLC | 説明 |
|---|---|---|
| エピック/サブドメイン | **ユニット(Unit)** | 凝集性のある自己完結型作業要素 |
| スプリント | **ボルト(Bolt)** | 時間/日単位の迅速な反復サイクル |
| 手動要件定義 | **モブエラボレーション(Mob Elaboration)** | AI主導の協調的要件精緻化セレモニー |
| 手動開発 | **モブ構築(Mob Construction)** | AI主導の協調的実装セレモニー |

## 3段階フレームワーク

```
インセプション(Inception) → 構築(Construction) → 運用(Operations)
```

- **インセプションフェーズ:** インテント(Intent)キャプチャおよびユニットへの分解
- **構築フェーズ:** ドメイン設計 → 論理設計 → コード生成 → テスト/検証
- **運用フェーズ:** デプロイ、観測可能性、AI基盤事前問題解決

## 10大コア原則

1. 改造ではなく再構想
2. 対話方向の逆転 (AIが主導、人間が検証)
3. 設計技法のコア統合 (DDD, BDD, TDD)
4. AI能力との現実的整合
5. 複雑なシステム構築の支援
6. 人間共生の向上を維持
7. 親しみやすさを通じた移行促進
8. 効率性のための責任簡素化
9. フェーズ最小化、フロー最大化
10. 固定されたSDLCワークフローなし

## 文書構造

```
.
├── AI-Driven Development Liftcycle.md   # 原本翻訳文書
├── index.md                              # GitHub Pages用 (韓国語)
├── CLAUDE.md                             # Claude Code作業ガイド
├── _config.yml                           # Jekyll設定
├── ja/                                   # 日本語版
│   ├── index.md                          # 日本語メイン文書
│   ├── README.md                         # 日本語概要
│   └── CLAUDE.md                         # 日本語ガイド
└── images/                               # ダイアグラムイメージ
    ├── ai-dlc-framework.png
    ├── ai-dlc-workflow.png
    └── ai-dlc-detailed-workflow.png
```

## GitHub Pages

本文書はGitHub Pagesでホスティングされる:
- 韓国語: https://serithemage.github.io/AI-DLC/
- 日本語: https://serithemage.github.io/AI-DLC/ja/

## 著作権

本文書のすべての権利は原著者(Raja SP, Amazon Web Services)に帰属する。本リポジトリは原文を日本語に翻訳したものである。

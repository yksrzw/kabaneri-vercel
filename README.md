# カバネリ海門決戦 設定推測カウンター

スマスロ甲鉄城のカバネリ 海門決戦の設定推測カウンターWebアプリです。

## Vercelへのデプロイ方法

### 方法A: GitHubリポジトリ経由（推奨）

1. このフォルダをGitHubリポジトリにpush
2. [vercel.com](https://vercel.com) にログイン
3. 「Add New Project」→ GitHubリポジトリを選択
4. そのまま「Deploy」をクリック（設定変更不要）

### 方法B: Vercel CLI

```bash
npm i -g vercel
cd kabaneri-vercel
vercel
```

プロンプトが出たらすべてデフォルト（Enter連打）でOK。

## ファイル構成

```
kabaneri-vercel/
├── public/
│   └── index.html    ← アプリ本体（単体HTML）
├── vercel.json       ← Vercel設定
└── README.md
```

## 機能

- 設定推測要素14カテゴリのカウント
- ベイズ推定による設定別確率分布の算出
- 確定演出の自動検知
- 全データのクリップボードコピー
- localStorageによるデータ永続化
- スマホ最適化UI（片手操作対応）

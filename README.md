# BOOKS Terminal

AI選書サービス。3つの質問に答えるだけで、あなたのためだけの5冊が届きます。

## セットアップ手順

### 1. GitHubにリポジトリを作る
- GitHubで `books-terminal` という名前のリポジトリを作成
- このフォルダの中身を全部アップロード

### 2. Vercelにデプロイする
1. https://vercel.com にアクセス
2. 「Continue with GitHub」でログイン
3. 「Add New Project」→ `books-terminal` を選択
4. 「Deploy」をクリック

### 3. APIキーを環境変数にセットする
1. Vercelのダッシュボード → プロジェクト → Settings → Environment Variables
2. 以下を追加：
   - **Name**: `ANTHROPIC_API_KEY`
   - **Value**: `sk-ant-xxxxxxxx`（自分のAPIキー）
3. 「Save」→「Redeploy」

### 4. 完成
発行されたURLにアクセスすると動きます。
そのURLをLINEのリッチメニューに貼れば連携完了です。

## ファイル構成
```
books-terminal/
├── index.html      # アプリ本体
├── api/
│   └── chat.js     # APIキーを安全に隠すサーバー側処理
├── package.json
└── README.md
```

## 費用目安
- Vercel: 無料プランで十分
- Anthropic API: 選書1回あたり約1〜2円

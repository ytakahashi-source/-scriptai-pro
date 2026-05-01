# ScriptAI Pro - Vercel公開手順

## 必要なもの
- Vercelアカウント（無料）→ https://vercel.com
- GitHubアカウント（無料）→ https://github.com

---

## 手順

### 1. GitHubにアップロード
1. https://github.com にログイン
2. 右上「＋」→「New repository」
3. Repository name に「scriptai-pro」と入力
4. 「Create repository」をクリック
5. 「uploading an existing file」をクリック
6. このフォルダの中身を全部ドラッグ＆ドロップ
7. 「Commit changes」をクリック

### 2. Vercelでデプロイ
1. https://vercel.com にログイン（GitHubアカウントで）
2. 「Add New Project」
3. 先ほど作ったGitHubリポジトリを選択
4. 「Deploy」をクリック
5. 数分待つと URLが発行される

### 3. APIキーを設定（重要）
1. Vercelのダッシュボードで対象プロジェクトを開く
2. 「Settings」→「Environment Variables」
3. 以下を追加：
   - Name: REACT_APP_ANTHROPIC_API_KEY
   - Value: （Anthropicで発行したAPIキー）
4. 「Save」→「Deployments」から「Redeploy」

### APIキーの発行場所
https://console.anthropic.com → API Keys → Create Key

---

## 公開後
発行されたURLをメンバーに共有するだけで使えます。
例：https://scriptai-pro.vercel.app

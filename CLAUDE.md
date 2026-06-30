# Olion Site - Project Guidelines

## 必須ルール（厳守）

### 実装完了後のデプロイ（最重要）

**実装作業が完了したら、必ず以下の手順でGitHub Pagesにデプロイすること：**

```bash
# 1. 変更をコミット
git add .
git commit -m "<type>: <description>

Co-Authored-By: Claude Opus 4.5 <noreply@anthropic.com>"

# 2. GitHubにプッシュ
git push origin main

# 3. GitHub Pagesにデプロイ
npm run deploy
```

**デプロイ後の確認:**
- 本番URL: https://jime0083.github.io/olion-site
- デプロイ完了後、上記URLで動作確認を行うこと

### デプロイタイミング

以下の作業完了後は**必ず**デプロイを実行：

| 作業内容 | デプロイ必須 |
|----------|-------------|
| 新機能の実装 | ✅ |
| バグ修正 | ✅ |
| スタイル変更 | ✅ |
| コンテンツ更新 | ✅ |
| 設定変更 | ✅ |

### チェックリスト

実装完了時に以下を確認：

- [ ] TypeScriptエラーがないこと (`npx tsc --noEmit`)
- [ ] ビルドが成功すること (`npm run build`)
- [ ] GitHubにプッシュ済み
- [ ] GitHub Pagesにデプロイ済み (`npm run deploy`)
- [ ] 本番環境で動作確認済み

## プロジェクト情報

- **フレームワーク**: React (Create React App)
- **言語**: TypeScript
- **デプロイ先**: GitHub Pages
- **本番URL**: https://jime0083.github.io/olion-site

## 開発コマンド

```bash
# 開発サーバー起動
npm start

# ビルド
npm run build

# TypeScriptチェック
npx tsc --noEmit

# GitHub Pagesデプロイ
npm run deploy
```

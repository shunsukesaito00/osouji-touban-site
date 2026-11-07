# 公開予定ファイル一覧（ホワイトリスト）

GitHub Pages にデプロイされる成果物は、ワークフローが `_site/` へコピーする次のファイルのみです。

## デプロイ対象（本番公開ファイル）

| パス | 内容 |
|---|---|
| `index.html` | アプリ紹介（ホーム） |
| `privacy/index.html` | プライバシーポリシー |
| `terms/index.html` | 利用規約 |
| `support/index.html` | サポート・FAQ |
| `404.html` | 404 ページ |
| `assets/css/site.css` | スタイル |
| `assets/img/favicon.svg` | ファビコン |

## リポジトリに含めるが Pages 成果物には載せないもの

| パス | 内容 |
|---|---|
| `.github/workflows/pages.yml` | デプロイ手順 |
| `.gitignore` | 無視設定 |
| `README.md` | リポジトリ説明 |
| `docs/FILE_WHITELIST.md` | 本一覧 |
| `docs/PREPUBLISH_CHECKLIST.md` | 公開前確認 |
| `docs/CONNECT_URLS.md` | App Store Connect 用 URL |

## 含めないもの（禁止）

- iOS / Swift ソースコード
- `ios-miniapp-factory` のミラーやサブモジュール
- CloudKit コンテナ ID、内部設計書、トークン、証明書
- App Store 提出用の内部チェックリスト原文（Private 側）
- 解析 SDK、不要な JavaScript バンドル

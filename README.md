# おそうじ当番 — 公式サイト

App Store 公開用のサポートサイト（静的 HTML/CSS）です。

- **Public リポジトリ**: 本リポジトリのみ
- **開発コード**: 含めません（Swift / Private `ios-miniapp-factory` とは分離）
- **ホスティング**: GitHub Pages（有効化は運営者の最終承認後）
- **言語**: 日本語
- **独自ドメイン**: なし

## ページ

| パス | 内容 |
|---|---|
| `/` | アプリ紹介 |
| `/privacy/` | プライバシーポリシー |
| `/terms/` | 利用規約 |
| `/support/` | サポート・FAQ |

想定公開 URL: <https://shunsukesaito00.github.io/osouji-touban-site/>

詳細は `docs/CONNECT_URLS.md` を参照。

## ローカル確認

静的ファイルのため、リポジトリルートを HTTP で開けば足ります。

```bash
# 例
python3 -m http.server 8080
# http://127.0.0.1:8080/
```

プロジェクトサイトと同じパス構成で試す場合:

```bash
mkdir -p /tmp/pages-root/osouji-touban-site
rsync -a --exclude .git --exclude docs --exclude .github ./ /tmp/pages-root/osouji-touban-site/
python3 -m http.server 8080 --directory /tmp/pages-root
# http://127.0.0.1:8080/osouji-touban-site/
```

## デプロイ

`.github/workflows/pages.yml` が `main` への push でホワイトリスト済みファイルを Pages にデプロイします。

**まだ GitHub Pages は有効化しないでください。** 有効化手順は運営者承認後に実施します。

1. Settings → Pages → Source: **GitHub Actions**
2. `main` に push、または workflow_dispatch
3. HTTPS で各 URL を確認

## 連絡先

- 運営: shunsuke saito
- メール: infomationshunsuke@gmail.com

## ドキュメント

- `docs/FILE_WHITELIST.md` — 公開ファイル一覧
- `docs/PREPUBLISH_CHECKLIST.md` — 公開前確認
- `docs/CONNECT_URLS.md` — Connect 用 URL

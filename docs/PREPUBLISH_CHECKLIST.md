# 公開前の確認事項

> Pages 有効化・一般公開の前に人手で確認する。虚偽の完了にしない。

## 機密・個人情報

- [x] Private 開発リポジトリを Public に変更していない
- [x] Swift ソースを含めていない
- [x] CloudKit コンテナ ID（例: `iCloud.com...`）を HTML に書いていない
- [x] GitHub トークン／秘密鍵をハードコードしていない
- [x] 運営者名は確定情報「shunsuke saito」を使用
- [x] 問い合わせ先は確定情報 `infomationshunsuke@gmail.com` を使用
- [ ] メールアドレスの綴りが意図どおりか最終確認（`infomation` の表記）
- [ ] 所在地の詳細をサイトに載せない方針で問題ないか（利用規約に TODO あり）

## 文章の正確性

- [x] ローカル保存を主とする説明
- [x] 通知はローカル／任意である説明
- [x] JSON 書き出し・取り込み・全削除の説明
- [x] 同一端末メンバーと、別 Apple ID 共有を混同しない
- [x] 別 ID 共有は「実験的・公開版で変わる場合あり」と記載（コンテナ等の内部識別子は非掲載）
- [x] 未実装機能（有料課金、広告、Web アカウント等）を宣伝していない
- [ ] App Store 公開後にダウンロード URL をホームへ追記
- [ ] 公開ビルドで共有 UI を除外した場合、プライバシー／利用規約の該当節を更新

## 技術

- [x] 相対リンクでホーム／privacy／terms／support を接続
- [x] 解析 SDK なし・追加 JS なし
- [x] デプロイはホワイトリスト方式
- [ ] GitHub Pages を Actions ソースで有効化（**ユーザー最終承認後**）
- [ ] HTTPS で各 URL にアクセスできることを確認（承認後）
- [ ] App Store Connect に PP URL・サポート URL を登録（承認後）

## Private リポジトリ側（別作業）

- [ ] `docs/app-store/OPEN_ITEMS.md` の運営者・メール・URL を本サイトに合わせて更新
- [ ] SUBMISSION_CHECKLIST の URL 欄を更新

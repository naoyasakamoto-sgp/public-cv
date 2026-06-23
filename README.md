# Detailed Public CV for Cloudflare Pages

顧客情報をマスキングした公開用スキルシート / CVです。

## 今回の方針

- 抽象的な「AIでできること」は記載しない
- 実際に担当した機能、技術、判断、意思決定を中心に記載
- 顧客名、企業名、プロダクト名、商流名はマスキング
- 技術詳細が不足する箇所には「⚠ 技術詳細要確認」を表示

## Cloudflare Pages 設定

- Framework preset: None
- Build command: exit 0
- Build output directory: .
- Root directory: 空欄 または /

## ファイル構成

- `index.html`：公開用CV本体
- `_headers`：noindex等のヘッダー
- `robots.txt`：検索エンジン除け
- `README.md`：このファイル

## 注意

`noindex` と `robots.txt` は検索エンジン対策であり、アクセス制限ではありません。
URLを知っている人には表示されます。完全に非公開にする場合は Cloudflare Access 等を利用してください。

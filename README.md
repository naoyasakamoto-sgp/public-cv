# 坂本直哉 公開用スキルシート / Cloudflare Pages

## 内容
このフォルダは、Cloudflare Pages にそのまま公開できる静的HTML一式です。

- `index.html`: 公開用CVページ
- `_headers`: 検索エンジンにインデックスさせないための HTTP ヘッダー
- `robots.txt`: クローラー向けの noindex 補助設定

## マスキング方針
以下は公開版から削除・匿名化しています。

- 顧客企業名
- 商流名
- 固有プロダクト名
- 顧客を特定しうる案件名
- 必要以上に細かい体制・内部運用情報

## Cloudflare Pages への公開方法

### 方法A: Direct Upload（最短）
1. Cloudflare ダッシュボードを開く
2. Workers & Pages → Create application → Pages
3. Direct Upload を選ぶ
4. このフォルダの中身をアップロード
5. 発行された `*.pages.dev` のURLを確認

### 方法B: Git連携（更新しやすい）
1. GitHubに新規リポジトリを作成
2. このフォルダの中身をコミット・push
3. Cloudflare PagesでGitHubリポジトリを接続
4. Build command は空欄、Output directory は `/` または未指定

## 注意
公開URLを共有する用途なら、検索エンジンに載せないため `noindex` 設定を入れています。
完全な非公開にしたい場合は、Cloudflare Access 等で認証を付けてください。

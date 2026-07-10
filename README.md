# らくシフト LP（リベライズ公開用）

介護シフト自動作成「らくシフト」のランディングページ一式です。
静的HTML（ビルド不要）。このフォルダの中身をそのままリポジトリに置けば公開できます。

## 構成

```
index.html            … LP本体
contact.html          … お問い合わせページ（送信は未接続・ボタン無効「準備中」）
assets/
  rakushift_logo.png    … ロゴ
  rakushift_favicon.png … favicon
  photos/jp-care-walk.jpg … 本文写真
```

パスはすべて相対参照なので、リポジトリ直下でもサブフォルダ（例 `/lp/`）配下でもそのまま動きます。
フォントは Google Fonts（BIZ UDPGothic / Klee One）を CDN 読み込みしています。

## 公開設定

**Cloudflare Pages の場合**
- Framework preset: `None`
- Build command: （空欄）
- Build output directory: `/`

**GitHub Pages の場合**
- Settings → Pages → Branch: `main` / `/ (root)`

## 公開前チェックリスト

1. **フッターのリンク先** `https://libelize.com/` がリベライズ社の正しいURLか確認
   （index.html / contact.html のフッター。同名の別会社があるため検索推定のまま）
2. **contact.html の送信先**（Googleフォーム or メール）を決めて接続
   （現状は見た目のみ。接続時に送信ボタンの disabled を解除）
3. 上記2件に対応したら、HTML内に残している `TODO` コメントを削除

## メモ

- ロゴ・favicon の PNG が約 0.8〜1MB と大きめです。表示速度が気になる場合は圧縮を推奨
- 写真は「おしごとピクチャーズ」素材（クレジット表記不要を規約で確認済み）

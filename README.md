# FrameSmoother 法務文書

iOS アプリ「FrameSmoother」のプライバシーポリシー・利用規約を公開するための GitHub Pages 用リポジトリです。

メインのコードリポジトリ: https://github.com/koheiomorijp/frame-smoother-app（Private）

## 公開 URL

独自ドメイン `framesmoother.naruberio.com` で公開している（KAN-1085。`CNAME`・`_config.yml` の `url`。DNS は naruberio-site の NaruberioAppPages）。
旧 URL（`https://koheiomorijp.github.io/framesmoother-legal/…`）は GitHub が同じパスへ 301 で転送するので（https への転送は Pages の「Enforce HTTPS」が有効なときだけ。切り替え後に `https_enforced` を確かめる）、アプリと App Store Connect の URL は変えていない。

- `sitemap.xml` は jekyll-sitemap が作る。`robots.txt` がその在りかを示し、Search Console（ドメインのプロパティ `naruberio.com`）と
  Bing Webmaster Tools に登録する
- `<32 桁の 16 進>.txt` は IndexNow の鍵（公開して使うもの）。ページを変えて公開したら、`keyLocation` をこのファイルにして IndexNow に通知する

公開 URL:

- プライバシーポリシー: https://framesmoother.naruberio.com/privacy
- 利用規約: https://framesmoother.naruberio.com/terms

## 言語

- 日本語（マスター）: `privacy-ja.md` / `terms-ja.md`
- 英語: `privacy.md` / `terms.md`（既定）

中国語・韓国語版は v1.1 以降で追加予定。

## 改訂方針

App Store 提出版と一致させる。改訂時はメインリポジトリ `frame-smoother-app/docs/legal/` も合わせて更新。

## サポート連絡先

konpei.work@gmail.com

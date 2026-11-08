# FrameSmoother 法務文書

iOS アプリ「FrameSmoother」のプライバシーポリシー・利用規約を公開するための GitHub Pages 用リポジトリです。

メインのコードリポジトリ: https://github.com/koheiomorijp/frame-smoother-app（Private）

## 公開 URL

GitHub Pages 有効化後、以下の URL で公開されます:

- プライバシーポリシー: https://koheiomorijp.github.io/framesmoother-legal/privacy
- 利用規約: https://koheiomorijp.github.io/framesmoother-legal/terms
- プライバシーポリシー（Android 版）: https://koheiomorijp.github.io/framesmoother-legal/privacy-android
- 利用規約（Android 版）: https://koheiomorijp.github.io/framesmoother-legal/terms-android

検索への登録:

- `sitemap.xml` は jekyll-sitemap が作る。Search Console の URL プレフィックス `https://koheiomorijp.github.io/framesmoother-legal/` へ送信する
- `5b6fcd19c442c187daf4197844659045.txt` は IndexNow の鍵（公開して使うもの）。ページを変えて公開したら、`keyLocation` をこのファイルにして通知する

## 用途別の説明ページ

検索や AI の回答から拾われる入口として、用途ごとに「比べて見せる」ページを置く。決まりと理由は frame-smoother-app の `docs/decisions.md` が正本。

| 用途 | en | ja | zh-Hans | `ct=` |
|---|---|---|---|---|
| 30fps → 60fps | `en/30fps-to-60fps/` | `ja/30fps-to-60fps/` | `zh-Hans/30fps-to-60fps/` | `web-60fps-en` / `web-60fps-ja` / `web-60fps-zh` |
| なめらかなスロー（2x・4x・8x） | `en/smooth-slow-motion/` | `ja/smooth-slow-motion/` | `zh-Hans/smooth-slow-motion/` | `web-slowmo-en` / `web-slowmo-ja` / `web-slowmo-zh` |
| アニメの重複コマ除去 | `en/anime-duplicate-frames/` | `ja/anime-duplicate-frames/` | `zh-Hans/anime-duplicate-frames/` | `web-anime-en` / `web-anime-ja` / `web-anime-zh` |

- 各ページは `index.html`（front matter は `layout: null`）。テーマを使わず `assets/compare.css` だけで描く。外部の JS・フォントは読まない
- canonical・hreflang・`og:url` は今の github.io の URL で書く。独自ドメインへ移すときは一緒に直す
- 画面の文言はアプリの表示（`Localizable.xcstrings` の en / ja / zh-Hans）とそろえる。アプリの文言を変えたらここも直す
- zh-Hans のページのフッターの法務のリンクは英語版を指す（法務文書に中国語版が無いため）
- App Store へのリンクは `https://apps.apple.com/app/apple-store/id6768623085?ct=<値>&mt=8`。`pt=` はまだ入れていないので、Analytics の Campaign には計上されない
- `sitemap.xml` には jekyll-sitemap が自動で載せる。ページを変えて公開したら IndexNow に通知する

## 言語

- 日本語（マスター）: `privacy-ja.md` / `terms-ja.md`
- 英語: `privacy.md` / `terms.md`（既定）
- Android 版: `privacy-android.md` / `terms-android.md`（英語）と `privacy-android-ja.md` / `terms-android-ja.md`（日本語）。iPhone 版とは別のページにする（購入・権限・保存の仕組みが違うため）

中国語・韓国語版は v1.1 以降で追加予定。

## 改訂方針

App Store 提出版と一致させる。改訂時はメインリポジトリ `frame-smoother-app/docs/legal/` も合わせて更新。

## サポート連絡先

konpei.work@gmail.com

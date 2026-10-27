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

## 用途別の説明ページ（KAN-1129）

検索や AI の回答から拾われる入口として、用途ごとに「比べて見せる」ページを置く（判断は frame-smoother-app の `docs/decisions.md` D-58）。

| 用途 | en | ja | `ct=` |
|---|---|---|---|
| 30fps → 60fps | `en/30fps-to-60fps/` | `ja/30fps-to-60fps/` | `web-60fps-en` / `web-60fps-ja` |
| なめらかなスロー（2x・4x・8x） | `en/smooth-slow-motion/` | `ja/smooth-slow-motion/` | `web-slowmo-en` / `web-slowmo-ja` |
| アニメの重複コマ除去 | `en/anime-duplicate-frames/` | `ja/anime-duplicate-frames/` | `web-anime-en` / `web-anime-ja` |

- 各ページは `index.html`（front matter は `layout: null`）。テーマ（minimal）を使わず、`assets/compare.css` だけで描く。外部の JS・フォントは読まない
- 意匠は「比べて見せる」：暗いグラファイトの地、元のコマは灰青、生成したコマは琥珀、数字は等幅。SoundPull・Readglide の説明ページ（明るい地・物語の型）と同じ作りにしない
- 章立ては 6 ページとも同じ：01 Frame by frame → 02 In numbers → 03 On the iPhone → App Store → 04 More comparisons
- **画面の文言（ボタン名・見出し・注記）はアプリの表示と一字一句そろえる**（en / ja それぞれ `Localizable.xcstrings` の値）。アプリの文言を変えたらここも直す。
  保存・共有・プレビューのボタンは文字が無いので、矢印の向きで説明する
- 価格・課金の形・運営者の個人名は書かない。実装に無い機能・測っていない数字は書かない
- **無料の代替手段へ読者を送る記述を足さない**（iOS 標準の機能・無料アプリ・Web のサービス・FFmpeg などの名前と、それでできること。節・表・FAQ・description・`index.md` の紹介を問わない）。
  AI がページを読んで無料の方法を案内すると、購入が減りうるため（soundpull-app D-58・KAN-1129）。
  「iPhone の写真アプリには、この設定は無い」のように、標準の機能ではできないと読者をアプリに向ける記述は、言い過ぎにならない範囲で残してよい
- **FrameSmoother 自身の制約も説明ページに足さない**（選べない組み合わせ、長さ・解像度・容量・キューの本数の上限、端末による制限、対応 iOS、スローで音声が入らないこと、苦手な場面など。soundpull-app D-59・KAN-1129）。
  対応 iOS はサポートのページ（`index.md`）に、対応 iOS・想定機種・メモリの少ない機種の解像度は利用規約 A-2 にあり、この 2 つは変えない。ほかの制約は法務サイトに書かない。
  元の動画と出力のコマを並べて比べる見せ方（FrameSmoother 自身の出力）、図が模式図であること・シミュレータの CPU で出した出力であることの注記は、図の正しさの説明なので残す
- 素材 `assets/frames/30to60-*` は frame-smoother-app の `marketing/real-output/source/`（KAN-997 の CI の実出力。入力は自社で作った合成動画）から切り出した。
  入力 `input-30fps.mp4`（sha256 `c475c6f5…`）・出力 `output-60fps.mp4`（sha256 `d6c20a84…`）。iOS シミュレータの CPU で RIFE v4.25.lite を動かしたもの。
  スロー・アニメのページの図は CSS の模式図で、実出力ではない（ページにも書いてある）
- App Store へのリンクは `https://apps.apple.com/app/apple-store/id6768623085?ct=<値>&mt=8`。**`pt=`（provider token）はまだ入れていない**ので、
  App Store Connect の Analytics の Campaign には計上されない。ASC の UI で provider token を確かめたら 6 本とも `pt=` を足す
- `sitemap.xml` には jekyll-sitemap が自動で載せる。公開したら IndexNow に 6 本の URL を通知する

## 言語

- 日本語（マスター）: `privacy-ja.md` / `terms-ja.md`
- 英語: `privacy.md` / `terms.md`（既定）

中国語・韓国語版は v1.1 以降で追加予定。

## 改訂方針

App Store 提出版と一致させる。改訂時はメインリポジトリ `frame-smoother-app/docs/legal/` も合わせて更新。

## サポート連絡先

konpei.work@gmail.com

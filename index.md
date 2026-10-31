---
layout: default
title: FrameSmoother
---

# FrameSmoother

An iPhone app that fills the gaps between video frames, entirely on the device, so motion plays back more fluidly.<br>
動画のコマの間を iPhone の中だけで補い、動きをなめらかにするアプリです。

## What it does / 何をするアプリか

FrameSmoother turns choppy video into smooth 60 or 120fps and slows it down without the stutter. It generates the in-between frames with AI on the iPhone itself, so your videos are never uploaded. Every feature comes with a single one-time purchase, with no subscription and no ads.

FrameSmoother は、カクつく動画をなめらかな 60fps・120fps にし、スローにしてもカクつかないようにするアプリです。間のコマを AI で iPhone の中だけで生成するので、動画をアップロードすることはありません。買い切りで、最初からすべての機能が使えます。サブスクリプションも広告もありません。

### Main uses / 主な用途

| Use / 用途 | What FrameSmoother does / FrameSmoother がすること |
|---|---|
| Smooth out choppy video / カクつく動画をなめらかに | Converts a video to a target frame rate (60 / 120fps) or by a multiplier (2x / 4x) by generating the frames in between.<br>目標の fps（60 / 120fps）か倍率（2x / 4x）を選ぶと、間のコマを生成して変換します。 |
| Smooth slow motion / なめらかなスローモーション | Slows a video down by up to 8x. Instead of repeating frames, it generates new ones, so motion stays fluid.<br>最大 8x までスローにします。同じコマを繰り返すのではなく間のコマを生成するので、動きが途切れません。 |
| Anime drawn on twos or threes / 2 コマ打ち・3 コマ打ちのアニメ | Removes the duplicate frames, then fills in the motion between drawings.<br>重複したコマを除いてから、絵と絵の間をなめらかにつなぎます。 |

Also: trim to process only the part you choose, stabilization to reduce camera shake in handheld footage, two quality modes (High Quality with AI / Fast without AI), a queue of up to 5 videos, a Before/After slider with frame-by-frame scrubbing, and export as mp4 or mov to Photos or AirDrop.<br>
ほかに、選んだ範囲だけを処理するトリム、手持ちで撮った揺れを抑える手ぶれ補正、補間品質 2 段階（高画質（AI）/ 高速（AI 不使用））、最大 5 本のキュー、フレーム単位でスクラブできる Before/After 比較スライダー、mp4 / mov での書き出し（写真に保存・AirDrop で共有）があります。

**[Get FrameSmoother on the App Store](https://apps.apple.com/app/id6768623085)** · **[App Store で FrameSmoother を入手](https://apps.apple.com/app/id6768623085)**

## What do you need? / ご用件

| If you want to… / こんなときは | Go here / 行き先 |
|---|---|
| know what happens to your videos and data / 動画やデータがどう扱われるか知りたい | [Privacy Policy](./privacy) · [プライバシーポリシー](./privacy-ja) |
| check the conditions for using and paying for the app / 使う条件や代金のきまりを確かめたい | [Terms of Service](./terms) · [利用規約](./terms-ja) |
| report a bug, sort out a purchase or ask a question / 不具合の報告、購入の相談、質問 | [konpei.work+framesmoother@gmail.com](mailto:konpei.work+framesmoother@gmail.com) |
| get your money back / 返金を申し込みたい | [reportaproblem.apple.com](https://reportaproblem.apple.com/) — Apple decides refunds, not the developer / 返金の可否は開発者ではなく Apple が決めます |
| download the app / アプリを入手したい | [App Store](https://apps.apple.com/app/id6768623085) — iPhone, iOS 16.0+ |

## Before you write / メールの前に

Adding your iPhone model, iOS version and the app version (near the bottom of FrameSmoother's Settings) speeds things up a lot. Replies normally come within about a week.

iPhone の機種、iOS のバージョン、アプリのバージョン（FrameSmoother の設定画面の下のほうにあります）を書き添えていただくと、調べるのがぐっと早くなります。返信にはおおむね 1 週間ほどいただいています。

---

Published by Kohei Omori, sole proprietor, Japan / 提供：大森 康平（個人事業主）

{% comment %}
構造化データ（KAN-1162）。検索エンジンと AI の回答に「何のアプリか」を渡すため。
価格（offers）は値段を変えるたびにページを直すことになるので入れない。評価（aggregateRating）は件数がほぼ 0 なので入れない。
url は site.url から作る（独自ドメインに移っても書き換えずに済む。KAN-1085）。文面を変えたら dateModified も変える。
{% endcomment %}
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "FrameSmoother",
  "alternateName": ["FrameSmoother: 60fps SlowMo", "FrameSmoother: 60fps スロー"],
  "operatingSystem": "iOS",
  "applicationCategory": "MultimediaApplication",
  "description": "An iPhone app that turns choppy video into smooth 60 or 120fps and makes smooth slow motion up to 8x by generating the in-between frames with AI on the device. It also removes duplicate frames from anime drawn on twos or threes. Videos are processed locally and never uploaded. One-time purchase, no subscription, no ads.",
  "featureList": [
    "Convert to a target frame rate (60 / 120fps) or by a multiplier (2x / 4x)",
    "Slow motion up to 8x with generated in-between frames",
    "Remove duplicate frames from anime drawn on twos or threes",
    "Trim to process only the part you choose",
    "Stabilization: reduce camera shake in handheld footage",
    "Two quality modes: High Quality (AI) and Fast (no AI)",
    "Queue up to 5 videos",
    "Before/After comparison slider with frame-by-frame scrubbing",
    "Export as mp4 or mov, save to Photos or share with AirDrop"
  ],
  "inLanguage": ["en", "ja"],
  "url": "{{ page.url | absolute_url }}",
  "downloadUrl": "https://apps.apple.com/app/id6768623085",
  "installUrl": "https://apps.apple.com/app/id6768623085",
  "sameAs": "https://apps.apple.com/app/id6768623085",
  "dateModified": "2026-10-31"
}
</script>

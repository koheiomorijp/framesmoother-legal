---
layout: default
title: FrameSmoother Privacy Policy
---

# FrameSmoother Privacy Policy

Effective date: **October 2, 2026** · [日本語](./privacy-ja)

This policy covers FrameSmoother, an iPhone app that generates in-between frames so that motion in a video looks smoother. It is issued by Kohei Omori, a sole proprietor in Japan who develops and sells the app; "I" and "me" below mean him. Instead of listing data categories, the policy takes each party that could conceivably see something and states what, if anything, reaches them.

## Who sees what

| Party | What reaches them | When |
|---|---|---|
| Your iPhone | Everything you work on: the clips you pick, the frames the app creates, the finished files, your preferences | Always. Processing does not leave the device |
| Apple | Purchase and ownership checks made through StoreKit; crash data only if you allow it in iOS | At launch, and when you buy or restore |
| Me, the developer | Sales totals from App Store Connect; reviews you post on the App Store; your message if you email me; Apple's crash data if you allow it | Only in those four cases |
| Apps and services you share to | The finished file you hand them | When you use the share sheet |
| Anyone else | Nothing | — |

### Your iPhone

You choose clips in Apple's photo picker, and FrameSmoother receives only the files you tick there. Each picked file is copied into a temporary folder that only FrameSmoother can open, inside the iPhone's app sandbox. A Core ML model bundled with the app, based on the open-source RIFE project, builds the new frames from that copy without any network connection. The finished video is written as a separate file; your original in Photos is never altered.

### Apple

Every exchange with Apple goes through the StoreKit framework, and the app opens no other connection. At launch, StoreKit reports which build of FrameSmoother you first downloaded and whether your Apple Account owns the Lifetime unlock; that answer decides whether the unlock screen is shown. Buying or restoring is likewise completed between StoreKit and the App Store. Card numbers, billing addresses and Apple Account details stay with Apple, which handles them under the [Apple Privacy Policy](https://www.apple.com/legal/privacy/).

### Me, the developer

App Store Connect gives me aggregated figures such as unit counts, countries and proceeds. It does not tell me who bought the app. If you post a review on the App Store, I read its nickname, country and text just as other visitors can, and I may reply to it through App Store Connect. If you email the support address, your email address, your message and any attachments arrive in my mailbox. I use them only to handle your enquiry and to investigate, fix and improve the app, and I neither add you to a mailing list nor forward your message to anyone. As a record of what was done, I may keep a summary with your name and email address removed in the issue tracker I use for development. Apple may also send me crash data and usage statistics for FrameSmoother, but only when you have enabled the iOS option described under "Permissions and switches" below; those reports are produced by iOS, not by the app. Nothing in the app or in iOS sends me your videos, file names or settings, apart from anything you attach to an email yourself.

### Apps and services you share to

Sending a finished video through the iOS share sheet gives it to whichever app or service you pick, and from then on that destination's own privacy terms apply. The links in the app to this policy, the terms, the open-source licences and support open in Safari or your mail app. This site is served by GitHub Pages, so visits to it fall under [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

### Anyone else

FrameSmoother contains no third-party code for analytics, advertising, attribution or crash collection, and it offers no account or sign-in. Its privacy manifest (`PrivacyInfo.xcprivacy`) declares no tracking and no collected data types, and the App Store privacy label reads "Data Not Collected".

## Permissions and switches you control

| Control | Where you set it | What it does |
|---|---|---|
| Photos: "Add Photos Only" (`NSPhotoLibraryAddUsageDescription`) | Asked by iOS the first time you save; change it later in iOS Settings → Privacy & Security → Photos | Lets the app place new videos in your library. It cannot read what is already there. Without it, finished files can still be shared |
| Auto-save to Photos | FrameSmoother → Settings. Off until you switch it on | Saves each finished video to Photos automatically |
| Share With App Developers | iOS Settings → Privacy & Security → Analytics & Improvements | Decides whether Apple passes crash data and usage statistics for the app on to me |
| Ask to Buy / purchase limits | Family Sharing, or Screen Time | Lets a parent approve or block purchases |

FrameSmoother never asks to browse your photo library, so items you do not pick stay out of its reach.

## How long things last

| Item | Kept until |
|---|---|
| Working copy of a clip you picked, and a finished output inside the app | iOS clears the app's temporary folder, or you delete the app. Copies you saved to Photos or shared are then yours to manage |
| Unfinished output of a job you stopped | Deleted when you stop the job |
| Preferences (default frame rate, file format, export quality, file-name prefix, auto-save, completion notice) and the flag that the intro screens were seen | You change them in Settings, or delete the app |
| Speed figures under Settings → Diagnostics | "Reset Samples", or the app quits. They are held in memory only |
| Short technical messages in iOS's on-device log, such as a failed export or a purchase that could not be verified | iOS rotates them. The app never transmits them; they reach me only if you export a diagnostic report yourself and send it |
| Whether you have paid | Never stored by the app. StoreKit is asked each time, so refunds and restores take effect correctly |
| Emails you send me | Until you ask me to delete them. The summaries kept in my issue tracker leave out your name and email address |

## Children

FrameSmoother is rated 4+. No part of it gathers information from anyone, children included. Because the app is paid, parents of children under 13 may want to turn on Ask to Buy or set purchase limits, as listed above.

## Requests about your data

The app sends me nothing, so I hold no app data about you that could be shown, corrected or erased. Emails are the exception: on request I delete them from my mailbox and remove anything that could identify you from the records in my issue tracker. Anything on the iPhone itself disappears when FrameSmoother is deleted.

## Revisions

A change in the law or in what the app does may require this policy to change. The effective date at the top moves with each revision, and important changes will be announced in the app or on this page. Should the app ever start collecting anything, this page will say so before the version that does it is released.

## Contact

Kohei Omori (sole proprietor, Japan)<br>
[konpei.work+framesmoother@gmail.com](mailto:konpei.work+framesmoother@gmail.com)

---

[Legal pages home](./) · [Terms of Service](./terms)

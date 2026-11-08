---
layout: default
title: FrameSmoother for Android Privacy Policy
permalink: /privacy-android
---

# FrameSmoother for Android — Privacy Policy

Effective date: **November 9, 2026** · [日本語](./privacy-android-ja) · iPhone version: [Privacy Policy](./privacy)

This page is about the Android edition of FrameSmoother, distributed through Google Play. FrameSmoother adds frames between the existing frames of a video so that its motion plays back more smoothly. The app is provided by Kohei Omori, a sole proprietor in Japan ("I", "me" below).

## In short

- The Android app has **no permission to use the internet**. It cannot send anything anywhere, and it does not.
- Videos are processed **inside your phone**. The AI model that creates the new frames ships inside the app.
- I **collect nothing** through the app: no analytics, no advertising code, no crash reporter, no account.

## What the app is built from

The permissions an Android app may use are fixed in its manifest and shown by Google Play. FrameSmoother's manifest requests five permissions, listed below (the three foreground-service permissions share a row), and `android.permission.INTERNET` is not among them:

| Permission | Why the app has it | What you see |
|---|---|---|
| Notifications (`POST_NOTIFICATIONS`) | To tell you that a video has finished, or that Android paused the work | On Android 13 and later, Android asks when you first start processing. Saying no does not stop the processing |
| Foreground service (`FOREGROUND_SERVICE`, with the `mediaProcessing` type on Android 15 and later, `dataSync` on Android 14 and earlier) | So that converting a video keeps going while you use other apps | A notification stays in the notification shade while a video is being processed, with its progress and a "Stop All" button |
| Wake lock (`WAKE_LOCK`) | So that the phone's processor does not fall asleep while a video is being processed and the app is not on screen | Nothing separate; it is released when the processing ends or is stopped |

The app also carries no third-party software development kit for analytics, ads or crash collection, and no Google Play billing library: you pay for FrameSmoother once in Google Play before installing it, and there is nothing to buy inside it.

## The path a video takes

1. **Choosing.** You pick a video in Android's photo picker, or send one to FrameSmoother from another app with Share. The picker hands over only the item you chose; FrameSmoother does not ask for permission to read your photo and video library.
2. **Copying.** The chosen file is copied into the app's private storage on the phone (a working folder other apps cannot open), because the link Android gives the app may stop working before processing ends.
3. **Processing.** A RIFE interpolation model bundled with the app, run by the ncnn library on the phone's graphics chip or, if that is not possible, its processor, generates the new frames from that copy. Your original file is left untouched.
4. **Result.** The finished video is written as a new MP4 file in the same private folder. From there it goes only where you send it: **Save to Gallery** places it in `Movies/FrameSmoother` on your phone (no storage permission is needed for this on Android 10 and later), and **Share** passes it to the app you choose, whose own privacy terms then apply.

## How long things stay on the phone

| What | Removed when |
|---|---|
| The working copy of a chosen video and an unsaved result | You remove the video from the queue, or the next time the app starts. Unsaved results do not survive the app being closed, which the app warns you about |
| A result you saved to the gallery or shared | It is no longer the app's: you manage it in your gallery or in the app you shared it with |
| Your settings (default frame rate, file-name prefix, auto-save, notifications) and the record that you have seen the intro screens | You change them, clear the app's storage, or uninstall the app |

Cloud backup is switched off for FrameSmoother. When you move to a new phone with Android's device-to-device transfer, your settings may come along; the working folder with videos is excluded from that transfer.

## Google

FrameSmoother is sold and delivered by Google Play. Paying for it, refunds, your Google Account and the information Google gathers when you use Google Play are handled by Google under the [Google Privacy Policy](https://policies.google.com/privacy). The app itself exchanges nothing with Google. Google Play gives me anonymous figures such as installs, countries, sales and crash or freeze counts (Android vitals); these come from Google Play and Android, not from anything the app sends, and they do not tell me who you are.

## Me, the developer

I receive your information in only two situations: when you email the support address below (your address, your message and anything you attach), and when you post a review on Google Play (the name and text shown publicly there, which I may answer). I use what you send to deal with your enquiry and to fix and improve the app. I do not put you on a mailing list or pass your message on. Development notes that I keep about a reported problem leave out your name and email address.

The links to this page, the terms and the support email open in your browser or email app. These pages are hosted on GitHub Pages; visiting them is covered by [GitHub's privacy statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Children

Because the app does not collect information from anyone, it does not collect information from children either. Parents can use Google Play's parental controls and purchase approval to manage whether a child can buy the app.

## Your requests

Since the app sends me nothing, I have no app data about you to show, correct or delete. If you have emailed me, I will delete your messages on request. Everything the app keeps on the phone is removed when you uninstall it.

## Updates to this policy

If the app or the law changes in a way that affects this policy, this page will be revised and the effective date above updated. If a future version of the app ever needs internet access or begins to collect anything, this page will say so before that version is released.

## Contact

Kohei Omori (sole proprietor, Japan)<br>
[konpei.work+framesmoother@gmail.com](mailto:konpei.work+framesmoother@gmail.com)

---

[Legal pages home](./) · [Terms of Service for Android](./terms-android)

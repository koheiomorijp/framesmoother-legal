---
layout: default
title: Privacy Policy
---

# Privacy Policy

**Last updated: May 12, 2026**

Kohei Omori (a sole proprietor, hereinafter the "Operator", "we", "us", or "our") provides this Privacy Policy to explain how we handle your information in the iOS application "**FrameSmoother**" (the "App").

---

## 1. Core principle

The App performs **all video processing entirely on your device**. Video files you select and processing results are never transmitted to our servers or any third-party servers. We do **not collect personal information** through the App.

## 2. Information we collect

The App does not collect any personal information, as detailed below.

| Information category | Collected? | Reason |
|---------------------|:---------:|--------|
| Name, email, contact info | ✗ Not collected | No account features |
| Video files, photos | ✗ Not collected | On-device processing only, no external transmission |
| Location data | ✗ Not collected | Not required by functionality |
| Device identifiers, advertising IDs | ✗ Not collected | No tracking |
| Usage history, operation logs | ✗ Not collected | No analytics |
| Crash reports | ✗ Not collected | Not supported in v1.0 (under consideration for v1.1+, separate notice will be issued) |

We declare "No Data Collected" in the App Privacy Manifest (`PrivacyInfo.xcprivacy`) to Apple.

## 3. Permissions used on device

The App uses only the following standard iOS permissions, with your explicit grant.

| Permission | Purpose | Info.plist key |
|-----------|---------|---------------|
| Add to Photos | To save interpolated video output to your Photos library | `NSPhotoLibraryAddUsageDescription` |

We do **not request read access to your photo library**. Video selection uses Apple's PHPicker (photo picker), which exposes only the videos you explicitly select to the App.

## 4. Communication with third parties

The App does not communicate over the network **except** for the following.

| Recipient | Purpose | Information transmitted |
|-----------|---------|------------------------|
| Apple StoreKit / App Store servers | In-app purchases (one-time and subscription) | Billing information managed automatically by Apple. We do not access this information. |

No third-party analytics services (Google Analytics, Firebase, etc.), advertising SDKs, or crash reporting services are integrated into the App.

## 5. In-App Purchases

The App offers digital content through Apple's App Store In-App Purchase (IAP) feature. Billing and payment information are handled **directly by Apple**, and we cannot access payment details (credit card numbers, etc.).

For more information, please refer to Apple's Privacy Policy (https://www.apple.com/legal/privacy/).

## 6. Children's use

The App is rated 4+, but for in-app purchases by children under 13, we recommend parents use Apple ID parental controls (Family Sharing, Screen Time) to manage usage.

## 7. Your rights

Since the App does not collect your information, we do not hold any data subject to disclosure or deletion requests.

The following information stored on your device can be deleted by you through iOS Settings or the App's "Settings" screen:

- App settings (default interpolation factor, filename prefix, etc.)
- Free export counter
- Temporary files from interpolation processing (automatically deleted within 100ms of completion or cancellation)

## 8. Changes to this Policy

This Policy may be revised due to legal changes or feature updates to the App. Significant changes will be notified within the App or on this page.

## 9. Contact

For inquiries regarding this Policy or how the App is operated, please contact:

- **Entity**: Kohei Omori
- **Email**: [konpei.work@gmail.com](mailto:konpei.work@gmail.com)

---

[← Home](./)

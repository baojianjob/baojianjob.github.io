---
layout: page
title: DarkBox Privacy Policy
permalink: /jiange-legal/privacy-en/
---

# DarkBox Privacy Policy

**Effective date: August 23, 2026**  
**Version: v1.0**

---

## TL;DR

DarkBox is a **fully local** encrypted app. We **do not collect** any personal information, we **have no servers**, and we **do not transmit** any of your data to us or to any third party. Everything you put into DarkBox is encrypted before it ever leaves the screen, and it stays only on your own device.

If you only read one paragraph, read that one. The rest of this document is the detailed version.

---

## 1. Scope

This policy applies to the mobile application **DarkBox** (the "App"), developed and published by the individual developer **baojianjob**. It describes how the App handles information related to you when you use it.

The App is intended for general adult users who want to store personal photos, videos and documents encrypted on their own device. It is not designed for children under the age of 13.

## 2. What we do NOT collect

Unlike most mobile apps, the App **does not collect any of the following**:

- Account information: no sign-up, no phone number, email, real name or government ID
- Device information: no IDFA / IDFV, device model, OS version, carrier or IP address
- Location information: no location permission is ever requested
- Contacts / Calendar / Microphone / Camera: not requested, not used
- Usage behavior: we do not track which files you open, how long you view them, what you tap, or how often you use the App
- Crash logs or diagnostics: not collected, not reported
- Advertising or analytics identifiers: the App contains no advertising or analytics SDKs

Because we do not operate any servers, there is nowhere for such information to be sent even if it existed.

## 3. What the App processes locally on your device

The following data is processed **only on your own device**, purely to make the App work:

| Data | Purpose | Where it lives |
|---|---|---|
| Photos, videos and documents you import | Encrypted and stored as your private content | Local app sandbox (ciphertext) |
| The password you set | Used to derive the encryption key | **Not stored**; used briefly in memory when you enter it |
| In-app preferences (sort order, view mode, folder covers, …) | Remembers how you use the App | Local app sandbox |

**About your password**: your password is never saved by the App and never leaves your device. We only store data derived from it to verify that a password entered later is correct. This means:

> ⚠️ **If you forget your password, no one — including the developer of this App — can recover or reset it. All encrypted content will be permanently unreadable. Please make sure you remember your password.**

## 4. System permissions and how they are used

When needed, the App requests the following system permissions. All of them follow the rule "nothing happens unless you actively trigger it":

- **Photo Library (read)**: used only when you explicitly tap "Import from Photos", to read the photos and videos you select. The App **never** scans your library in the background, and it fully supports iOS "Limited Access" (you may grant access to selected photos only).
- **Photo Library (write)**: used only when you explicitly tap "Export to Photos", to save the items you selected back to the system library.
- **Files / Share Extension**: used only when you actively choose "Share to DarkBox" or "Open in DarkBox" from another app.

The App does **not** request any other permissions (camera, microphone, location, contacts, calendar, etc.).

## 5. Network behavior

The App **itself makes no network requests**. It does not phone home, sync, validate licenses over the wire, or fetch remote configuration.

The only network activity involved is **Apple's In-App Purchase (StoreKit)**: when you tap Subscribe or Buy inside the App, iOS itself talks directly to Apple's servers to complete the transaction and receipt validation. The App never sees your payment information and never sees your Apple ID. That part is covered by [Apple's privacy policy](https://www.apple.com/legal/privacy/).

**About system iCloud backup**: iCloud Backup is a feature that iOS provides to you. Whether it is turned on, and whether it includes the App, is controlled by you in **Settings → [Your Name] → iCloud → iCloud Backup**. If you enable it, iOS will include the App's data in **your own** iCloud backup — however:

- What gets backed up is **only the encrypted ciphertext**, not your original photos or documents;
- Your **password is not backed up** (we never stored it in the first place), so no one who obtains the backup — including Apple, or even you on another device — can decrypt anything without your password;
- This is **not** the App uploading data. The App has no network upload capability of its own; whether iOS backs it up is entirely your choice;
- If you do not want the App's data included in your backups, you can disable the App individually in the iCloud Backup settings above.

In other words: **"local encryption" guarantees that whenever your data leaves the device it is still ciphertext and the key is only in your head**. Whether that ciphertext travels with your own iCloud backup is up to you.

## 6. Storage and encryption

- All content is encrypted with **AES-256-GCM** in chunks before being written to disk.
- The encryption key is **derived from your password**, which never leaves your device.
- Metadata such as file names and folder structure is stored in an **encrypted local database**.
- Precise cryptographic parameters may evolve with future versions of the App and are governed by the App's source code, not by this document. However, we commit that **no future change will weaken the "local only, ciphertext only" property described above**.

## 7. Sharing and third parties

The App **does not integrate any third-party SDK** — no analytics, no advertising, no push notifications, no crash reporting.

We do not share, sell, transfer or disclose any of your data to any third party, because we simply do not have any of your data to share.

## 8. Exporting and deleting your data

- **Export**: at any time you may use features such as "Export to Photos" to move content out of the App to your device or to another app. Once exported, the file is handled by iOS or by the destination app, and its safety is governed by that party's rules.
- **Delete**: you may delete any file or folder from within the App. **Uninstalling the App** causes iOS to erase all of the App's local data. We keep no backups on our side.

Because we do not hold any of your data, the rights to "access, correct, delete or withdraw consent" apply to the data that lives locally on your device. You can exercise these rights entirely through in-app actions or by uninstalling the App — no request to us is needed.

## 9. Children's privacy

The App is not designed for children under 13 and does not knowingly collect any personal information from children. If you are the guardian of a minor and believe a child used the App without your consent, please contact us via the address below.

## 10. Changes to this policy

If future functionality requires changes to this policy (for example, an optional cloud backup feature), we will:

1. Update the "Version" and "Effective date" at the top of this document;
2. Ship the new policy as part of an App update;
3. For **material changes** (i.e. any new way of handling data), display a clear notice inside the App, and keep the related feature turned off by default until you enable it yourself.

## 11. Contact

If you have any questions, comments or complaints about this policy, please contact:

**baojianjob@vip.qq.com**

We will do our best to respond within a reasonable time.

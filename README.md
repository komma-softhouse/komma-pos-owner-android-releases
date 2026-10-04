# Pyme for Android

**Photograph a supplier invoice. Find the expense draft waiting in your panel.**

This is the official download page of the Pyme capture app for Android, by [Komma SoftHouse](https://kommasofthouse.com). Pyme is the invoicing product for small businesses with VERI\*FACTU, TicketBAI and FACe built in: [pyme.kommasofthouse.com](https://pyme.kommasofthouse.com).

[**Download the latest version**](https://github.com/komma-softhouse/pyme-app-android-releases/releases/latest)

---

## What the app does

| | |
|---|---|
| **Capture** | Take a photo of a supplier invoice or ticket, or pick one from the gallery. |
| **Read** | Pyme reads supplier, date, lines and taxes and creates an expense draft. If the reading does not match the printed total, nothing is created and the app tells you why. |
| **Review** | The draft waits in Expenses in your panel. You check it and book it. Nothing is booked on its own. |
| **Offline** | No coverage at the counter or in the van? The capture waits on the phone and is sent on its own when the signal returns. |
| **Follow** | Every capture shows where it stands: waiting for network, being read, draft created, or not created with the reason. |
| **Several businesses** | If your account has more than one issuer, choose which one receives each capture. |

## Screenshots

| Pairing | Capture | Sent | Settings |
|---|---|---|---|
| ![Pairing](assets/01-pair.jpeg) | ![Capture](assets/02-capture.jpeg) | ![Sent](assets/03-sent.jpeg) | ![Settings](assets/04-settings.jpeg) |

## Before you start

- A Pyme account with a plan that includes expenses and photo readings.
- An Android phone with a camera and an internet connection.

No account yet? [Create one](https://pyme.kommasofthouse.com/signup).

## Install

1. On the phone, open the [latest release](https://github.com/komma-softhouse/pyme-app-android-releases/releases/latest) and download `Pyme-<version>.apk`.
2. Open the downloaded file.
3. Android asks whether to allow installing apps from your browser. Allow it; you can switch it off again afterwards.
4. Press **Install**, then **Open**.

## Pair the phone with your account

1. In your Pyme panel, open **Pyme → Mobile app** and press **Pair a phone**. A QR code appears.
2. In the app, press **Scan the pairing code** and point at the QR.
3. The phone is linked to your account. The code works once and expires after 15 minutes.

No camera at hand for the QR? Press **Type it instead** and enter the address of your panel and the code shown under the QR.

## Send your first invoice

1. Choose **Invoice** or **Ticket**.
2. Press **Take the photo**. Keep the whole document inside the frame, flat and well lit.
3. In a few moments the capture shows **Draft in Expenses**.
4. In your panel, open **Expenses**, review the draft and book it.

## Updates

The app updates itself from this page. Open **Settings → Updates → Check for updates**; when a new version exists, the app downloads it, checks it and opens the installer.

The first time, Android asks you to allow Pyme to install updates. The app takes you to that permission.

## Check your download

Every release publishes the SHA-256 of its APK next to it (`Pyme-<version>.apk.sha256`). To check a file downloaded to a computer:

```bash
shasum -a 256 Pyme-<version>.apk
```

The result must match the published one. All versions are signed with the same key, so Android refuses any file that does not come from Komma SoftHouse as an update of the installed app.

## Permissions

| Permission | Why |
|---|---|
| Camera | To photograph documents and to scan the pairing QR. |
| Photos | Only when you pick a document from the gallery. |
| Internet | To send captures to your own panel. |
| Install apps | Only for the app to install its own updates. |

## Your data

- The app talks only to the address of your own panel, over HTTPS.
- The address and the access key of the phone are kept in the secure storage of the device.
- A photo stays on the phone only until your panel confirms the draft. Then it is deleted from the phone.
- Unpairing, from the app or from your panel, cuts the access at once and clears what the app had stored.

## Problems

**"That code is not valid or has expired"** — Codes last 15 minutes and work once. Press **Pair a phone** again in your panel and scan the new one.

**"No connection to …"** — Check the phone has internet and, if you typed the address, that it is the address of your own panel.

**A capture says "Not created"** — The reason is written under it. The usual ones: the photo is blurred or cut, the totals do not match what is printed, or your plan has no readings left this period. Take the photo again or press **Send again**.

**A capture stays in "Waiting for network"** — Open the app with coverage; it is sent on its own.

**The app asks to pair again** — The phone was unpaired from the panel. Pair it again; what it had already sent is still in your panel.

**Android does not let me install** — Allow installing from your browser when Android asks, or look for "Install unknown apps" in the phone settings.

## Versions

Every version, with its changes, is listed in [Releases](https://github.com/komma-softhouse/pyme-app-android-releases/releases).

## Support

info@kommasofthouse.com

Something went wrong inside the app? The error screen has a **Report the error** button that sends us what happened with a code you can quote.

## Licence

Proprietary software. © Komma SoftHouse. This repository holds only the signed builds; the source code is not public.
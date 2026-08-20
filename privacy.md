---
title: Privacy Policy
---

# Privacy Policy

**Last updated: 9 August 2026**

Veilbox does not collect, transmit, or sell any personal information. There are
no accounts, no analytics, no advertising, no tracking, and no crash reporting.

This policy is short because there is genuinely very little to say.

## What stays on your iPhone

Everything, unless you turn on iCloud backup. The following are stored on your
own device and are never sent anywhere:

- Your photos and videos, encrypted with AES-256
- Your vault code — stored only as a one-way hash, never in readable form
- Your encryption keys, held in the iOS Keychain
- Albums, dates, and app settings

## What happens if you turn on iCloud backup

Encrypted data is copied to **your own** iCloud account, in a private database
only your Apple Account can reach. We have no server and receive nothing.

Everything uploaded is encrypted on your iPhone first. That includes the
metadata: album membership, dates, and deletion state are sealed too, because
the way a vault is organised is itself revealing. Apple stores the data but
cannot read it, and neither can we.

Your vault code is never uploaded. What is uploaded is your encryption key
wrapped under a key derived from that code (PBKDF2-HMAC-SHA256, 600,000
rounds). Without the code it is unusable ciphertext. This is what lets the same
code open your vault on a new phone — and it is why a forgotten code cannot be
recovered by anyone.

## Photo library access

Veilbox asks for permission to read photos only when you import, and only
add-only permission when you export back to your camera roll. It never browses
your library on its own.

## Camera access

Only if you enable the break-in log, which photographs whoever enters a wrong
code. Those photos are encrypted in your vault and never leave your device
unless you have backup on. iOS always shows the green camera indicator when the
camera is used; that cannot be turned off, and we would not want it to be.

## Purchases

In-app purchases are handled entirely by Apple. We never see your payment
details. Veilbox asks Apple whether a purchase is active and nothing more.

## Keeping and deleting your data

Apple's App Review Guidelines require every privacy policy to say how long data
is kept and how you get rid of it. For Veilbox that is unusually simple, because
almost none of it is ours to keep.

**On your iPhone.** Photos stay until you delete them. A deleted photo goes to
Recently Deleted and is recoverable for 30 days, then erased permanently. You can
empty that folder immediately from inside the app. Deleting the app removes
everything it stored on the device.

**In iCloud.** Only if you turned backup on, and only into *your own* iCloud
account — we have no server and receive nothing. Settings → Danger zone →
**Remove everything from iCloud** deletes the cloud copy and turns backup off,
leaving the photos on your phone untouched. This is free and does not require a
subscription.

**Getting your data out.** Settings → **Export photos** saves everything, or one
album, back to your camera roll. Also free, and always will be — a subscription
that lapsed can never strand your own photos.

**Withdrawing permission.** Photo library and camera access can be revoked at any
time in the iOS Settings app under Veilbox. The app keeps working; it simply
stops being able to import or capture.

**What we hold.** Nothing. There is no account, no server, and no analytics, so
there is no record of you to request the deletion of.

## Children

Veilbox is not directed at children and collects no data from anyone.

## Changes

If this policy ever changes, the date at the top changes with it. The full
history is public in the [repository for this site](https://github.com/JosueC33/veilbox-site).

## Prefer slides?

The same policy, as a short deck: [Privacy, in 8 slides](privacy-deck.html).
This page remains the canonical policy.

## Contact

[Open an issue on GitHub](https://github.com/JosueC33/veilbox-site/issues).

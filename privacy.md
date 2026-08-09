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

## Children

Veilbox is not directed at children and collects no data from anyone.

## Changes

If this policy ever changes, the date at the top changes with it. The full
history is public in the [repository for this site](https://github.com/JosueC33/veilbox-site).

## Contact

[Open an issue on GitHub](https://github.com/JosueC33/veilbox-site/issues).

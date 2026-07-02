# EclipsePro Privacy Policy

**Effective date:** June 30, 2026

EclipsePro ("the App") is a macOS application developed by Jon Mobley ("we", "us"). This policy describes what information the App accesses, how it is used, and what (if anything) leaves your computer.

## Summary

EclipsePro is a local-first application. We do not operate accounts, collect analytics, or run servers that receive your content. Your media, settings, and screen content stay on your Mac except in the limited cases described below.

## Information the App accesses

### Camera and microphone
With your permission, the App accesses connected cameras (and microphones for video capture) to display live feeds on external screens. Camera and microphone data is processed in real time on your Mac and is never transmitted to us.

### Screen recording
With your permission, the App captures your desktop and application windows so they can be shown on external displays. Captured screen content is processed in memory on your Mac and is never stored or transmitted to us.

### Media files
Images, videos, and slideshows you import are copied into folders inside your local Documents directory. They remain on your Mac.

### PowerPoint automation
If you enable the Hide Presenter View feature, the App uses macOS Automation (Apple Events) to reposition Microsoft PowerPoint's Presenter View window. No presentation content is read or transmitted.

## Information that leaves your Mac

### Web page browsing
When you add or open a web page, the App loads it in an embedded browser, which communicates directly with that website and any third parties it contacts. Those sites are governed by their own privacy policies. Browsing data (cookies, logins, cache) is stored locally by the system browser engine.

### Software updates
The App periodically checks for updates using the Sparkle framework. Update checks contact GitHub (where releases are hosted), which receives standard request information such as your IP address. No personal data is included in update checks.

### Local network (EclipseCast)
If you use EclipseCast, the App discovers and communicates with receiver devices (such as an Apple TV running EclipseTV) over your local network using Bonjour and TCP. Pairing tokens are stored securely in the macOS Keychain. This traffic stays on your local network.

### Licensing
To validate your license, the App contacts our licensing service (Keygen) over the network, sending your license key and a hardware-derived machine fingerprint so a license can be locked to your Mac. A signed validation receipt is cached in the macOS Keychain so the App keeps working offline within a grace period. The license-recovery feature sends an email address you enter to our Cloudflare Worker so it can re-send your key; the email is only used to look up and re-send your key.

### Asset store
If you open the in-app Eclipse Store, the App fetches a catalog of available asset packs from our Cloudflare Worker. When you buy a pack, the App opens a Stripe Checkout page in your browser to complete payment; we never see or store your card details. Purchases are attached to your existing license as an entitlement (no separate account). When you install a pack, the App sends your license key to the Worker to authorize the download, then downloads the pack's files from Cloudflare R2.

Store assets are licensed to you, not sold as files: they are stored encrypted on your Mac, decrypted only in memory at playback time, and cannot be exported or included in exported presentation packages. The per-pack decryption key is stored in the device-only macOS Keychain. This is a deterrent against casual copying, not an absolute guarantee; content shown on screen can always be recaptured.

## What we do not do

- We do not collect analytics or telemetry.
- We do not sell or share your data.
- We do not require an account.
- We do not store your content on our servers.

## Data retention and deletion

All App data (imported media, preferences, pairing tokens, purchased store assets) is stored locally. Deleting the App and its data folders (`~/Documents/Images`, `~/Documents/Videos`, `~/Documents/Slideshows`, `~/Documents/Thumbnails`, `~/Documents/StorePacks`) removes your content. Preferences can be removed by deleting the App's entries in `~/Library/Preferences`, and pairing tokens, the license receipt, and store decryption keys via Keychain Access.

## Children's privacy

The App is not directed at children under 13 and does not knowingly collect personal information from anyone.

## Changes to this policy

We may update this policy from time to time. Material changes will be noted in release notes and the effective date above will be updated.

## Contact

Questions about this policy? Contact: **jon@jonmobley.com**

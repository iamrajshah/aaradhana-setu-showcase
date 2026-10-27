# AaradhanaSetu

> A multilingual, offline-first devotional companion that keeps daily practice, trusted reading, and personal collections close—even when the network is not.

<p align="center">
  <img src="assets/demo-cover.jpg" alt="AaradhanaSetu mobile app showing its devotional home experience" width="100%" />
</p>

<p align="center">
  <img alt="Ionic React" src="https://img.shields.io/badge/Ionic_React-Mobile-3880ff?style=flat-square&logo=ionic&logoColor=white" />
  <img alt="Capacitor" src="https://img.shields.io/badge/Capacitor-Android_%2B_iOS-119eff?style=flat-square&logo=capacitor&logoColor=white" />
  <img alt="Cloudflare" src="https://img.shields.io/badge/Cloudflare-Workers_%2B_D1_%2B_R2-f38020?style=flat-square&logo=cloudflare&logoColor=white" />
  <img alt="Languages" src="https://img.shields.io/badge/Languages-Gujarati_%7C_Marathi_%7C_Hindi_%7C_English-7c3aed?style=flat-square" />
  <img alt="AI assisted" src="https://img.shields.io/badge/Engineering-AI_assisted-0f766e?style=flat-square" />
</p>

## The product

AaradhanaSetu brings Daily Darshan, deity-led discovery, devotional galleries, a multilingual PDF library, offline reading, favourites, recent history, and a Jaap counter into one calm mobile experience. It is designed for people who may have intermittent connectivity, prefer familiar language choices, and want devotion without a crowded content feed.

The application pairs a reader-facing mobile app with a private publishing system. Approved editors can manage localized titles, document versions, deity imagery, ordering, and publication status without shipping a new app release for every catalogue change.

## Download the app

📲 **[Get AaradhanaSetu on Google Play](https://play.google.com/store/apps/details?id=io.github.iamrajshah.aaradhanasetu)**

## Watch the product

▶️ **[Play the AaradhanaSetu app walkthrough](demo/AaradhanaSetu-app-demo.mp4)**

The silent walkthrough was captured from the current mobile app against the read-only published catalogue on 16 October 2026. It uses no third-party music, credentials, private administration screens, or live catalogue writes.

<p align="center">
  <img src="assets/product-overview.jpg" alt="AaradhanaSetu product walkthrough covering home, deity discovery, the library, offline access, and language options" width="100%" />
</p>

## Product walkthrough

### A devotional home, not another content feed

Daily Darshan, quick access to personal practice, and deity-led navigation give the app a clear starting point without overwhelming the reader.

<p align="center">
  <img src="assets/home-daily-darshan.png" alt="AaradhanaSetu home screen with Daily Darshan and devotional shortcuts" width="360" />
</p>

### Connected traditions and visual discovery

| Related collections | Darshan gallery |
| --- | --- |
| <img src="assets/related-collections.png" alt="Deity collection with related devotional traditions" width="360" /> | <img src="assets/darshan-gallery.png" alt="Darshan image gallery in AaradhanaSetu" width="360" /> |

Readers can move naturally between related deity collections, browse a focused gallery, swipe through imagery, and save a selected Darshan for personal use.

### A multilingual library that works offline

| Searchable catalogue | Offline collection |
| --- | --- |
| <img src="assets/full-library.png" alt="Searchable AaradhanaSetu library with language filters" width="360" /> | <img src="assets/offline-library.png" alt="Downloaded devotional books available offline" width="360" /> |

The library separates interface language from document language, supports search and filtering, and clearly shows what is downloaded and ready without a connection.

### Reading and personal practice

| Focused PDF reader | Jaap counter |
| --- | --- |
| <img src="assets/pdf-reader.png" alt="AaradhanaSetu devotional PDF reader" width="360" /> | <img src="assets/jaap-counter.png" alt="AaradhanaSetu Jaap counter for personal practice" width="360" /> |

Reading, favourites, recent history, downloads, and the Jaap counter are treated as personal tools—not engagement tricks.

### Four interface languages

<p align="center">
  <img src="assets/language-options.png" alt="Gujarati, Marathi, Hindi, and English language choices" width="360" />
</p>

Gujarati, Marathi, Hindi, and English are first-class interface choices, with document language retained as separate catalogue metadata.

## What I built

- A multilingual Ionic React application packaged for Android and prepared for iOS through Capacitor.
- Daily Darshan, deity relationships, devotional galleries, image saving, and a personal Jaap counter.
- An offline-first library with starter content, verified downloads, favourites, recently opened items, and a PDF reader.
- Remote catalogue synchronization with checksums and immutable content versions.
- A private React publishing portal for localized metadata, PDFs, imagery, visibility, and ordering.
- Cloudflare Workers APIs backed by D1 metadata and private R2 object storage.
- Short-lived delivery authorization so private documents are not exposed as permanent public URLs.
- Public privacy and support pages plus an Android release workflow.

## Product decisions that mattered

| Challenge | Decision |
| --- | --- |
| Unreliable connectivity | Keep starter documents in the app and cache approved downloads for offline reading |
| Four-language content | Treat display language and document language as separate, explicit metadata |
| Safe document updates | Publish immutable versions with checksums instead of overwriting files in place |
| Private content delivery | Authorize downloads through the API and issue short-lived storage access |
| Small trusted editorial team | Protect the publisher portal separately from the public reader experience |
| Mobile release friction | Make catalogue and metadata changes server-driven wherever native changes are unnecessary |

## Architecture

<p align="center">
  <img src="assets/architecture.svg" alt="AaradhanaSetu public architecture diagram" width="100%" />
</p>

The public diagram intentionally shows system boundaries without exposing live resource identifiers, credentials, private administration URLs, operational playbooks, or content files.

## AI-assisted engineering

AaradhanaSetu was built end to end with AI-assisted engineering and compound engineering practices: product discovery, architecture exploration, implementation, testing, multilingual content tooling, release preparation, and operational documentation. I remained responsible for product decisions, security boundaries, verification, and what was allowed to ship.

The useful lesson was not “AI wrote an app.” It was that disciplined AI collaboration can shorten the path from idea to a tested mobile product—provided every generated decision is reviewed against real constraints.

## Delivery status

- [Available on Google Play](https://play.google.com/store/apps/details?id=io.github.iamrajshah.aaradhanasetu) with the Android application ID and release-signing path established.
- The published mobile experience and catalogue are represented in the walkthrough above.
- The iOS project is generated and device testing is supported; App Store release work remains separate.

## Why the source repository is private

The production repository includes private infrastructure configuration, release and recovery procedures, publishing controls, and licensed or owner-supplied devotional content. Keeping that repository private is a security and content-rights decision, not an absence of working software.

This showcase contains no customer data, secrets, private URLs, source PDFs, or reusable credentials.

## About the builder

Built independently by [Rajesh Shah](https://github.com/iamrajshah), a lead engineer focused on product-minded backend, platform, mobile, and AI-assisted delivery.

Connect on [LinkedIn](https://www.linkedin.com/in/iamrajshah/).

---

This repository is a public product showcase. Source code and production assets are not licensed for reuse or redistribution.

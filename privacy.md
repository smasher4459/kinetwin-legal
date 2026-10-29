---
layout: default
title: Kinetwin beta privacy notice
description: Privacy notice for the Kinetwin TestFlight beta (version beta-notice-v2).
permalink: /privacy/
---

# Kinetwin beta: privacy notice

Version `beta-notice-v2` · dated 28 October 2026 · applies to consent version `kinetwin-beta-consent-2` · covers the Kinetwin TestFlight beta only

Published at https://smasher4459.github.io/kinetwin-legal/

Earlier versions stay available at the same address. In this notice "I" and "me" mean Simon Pastoor, the person responsible for your data. "Kinetwin" means the iPhone app.

## 1. The short version

- The beta exists to collect test data. **If you join, every clip you analyse is uploaded.** If you do not want that, do not join. You lose nothing by saying no.
- What goes up: your video (with the sound and the hidden information inside the video file removed), the body pose, 3D twin and measurements Kinetwin made from it, and some technical details about your phone and the video. If you add them, also your known 1RM, the weight of a set and a bar-velocity file.
- Your video can show your face and body. Anything stored under a random donor ID can still be about you, so it is **pseudonymised, not anonymous**.
- Only I can use it. I use it to improve Kinetwin and for research on lifting technique. I do not sell it, I do not show you ads, and the app contains no advertising or tracking code.
- Files are stored in a private storage area in the EU at Cloudflare, my service provider. They are deleted automatically after about 730 days (24 months), or earlier when you delete them in the app.
- You can delete your data or leave the beta at any time in **Beta settings**.

## 2. Who is responsible

| | |
|---|---|
| Controller | Simon Pastoor, an individual developer in the Netherlands |
| Contact for anything in this notice | kinetwin@proton.me (you may write in English or Dutch) |
| Data protection officer | None. Not required at this scale (GDPR Art. 37). |
| Supervisory authority | Autoriteit Persoonsgegevens (AP), the Dutch data protection authority |

## 3. What this notice covers

This notice covers the data the Kinetwin beta uploads when you join the TestFlight beta, and the other data I handle to run the beta (section 4.5). It does not cover:

- **Apple and TestFlight.** Apple runs TestFlight. Apple handles your invitation, your installs and its own crash and usage reports under Apple's own privacy policy (https://www.apple.com/legal/privacy/). Section 4.5 says what Apple passes on to me.
- **A later public Kinetwin app.** It will have its own notice and its own consent.

Your analysis runs on your phone. Nothing is uploaded until you tick both boxes and tap **Join the beta**.

## 4. What I collect

### 4.1 The files of each donation

After you finish with a clip, the app uploads these files. They are the only file names the server accepts.

| File | What it is |
|---|---|
| `clip.mov` or `clip.mp4` | Your video of the lift, up to 600 MB. The app removes the sound and the information stored inside the video file (such as GPS location, device make and model, software and recording date) before it uploads. The picture itself is not changed: it may show your face, your body, the room and other people near you. |
| `pose.json` | The 3D body pose the app measured in each frame (joint positions). |
| `twin.json` | The script of your 3D twin, the animated skeleton the app builds from your lift. |
| `metrics.json` | Up to six measurements calculated from the twin: bar vertical travel, the largest sideways offset of the bar, and the left and right elbow angles at the lowest and highest bar point, each with a note on how uncertain it is. |
| `meta.json` | Technical details, listed in 4.2. |
| `feedback.json` (optional) | Two numbers, only if you fill them in: your known one-repetition maximum and the weight of the set, in kilograms. No free text. |
| `velocity.csv` (optional) | A file you choose from the Files app, exported from a bar-velocity sensor. It is sent exactly as it is, without being read or changed. Remove names and other personal details from it before you choose it. |
| `velocity_meta.json` (optional) | The sensor brand you pick, the export date you pick and the number of rows in the file. |

### 4.2 What `meta.json` holds

- app version and build;
- device model;
- iOS version;
- region only (for example NL), not your full language setting;
- where the clip came from in the app (Photos or Files);
- video format: codec, size, frame rate, duration and rotation;
- the camera lens name (which can include your phone model) and its focal length, if your video file records them (never location or date);
- the height you typed, and where it came from;
- the Vision request revision and, per refusal reason, how many frames the pose analysis refused;
- the analysis time;
- the consent version.

### 4.3 Identifiers and records

- **Donor ID and token.** On first launch the app makes a random donor ID and keeps a random secret token in your iPhone Keychain. Your files are stored under the donor ID. The server keeps only a SHA-256 hash of the token, so that only your phone can order deletion.
- **A manifest for every donation** (`_manifest.json`). It lists the donor ID, a donation ID, when the donation was started and completed, the app version, the consent version and the time you consented, and, for each file, its name, size and checksum.
- **Counters.** A daily counter of how many donations your donor ID started, and markers for donations that have been started but not finished.
- **Consent record.** The app stores on your phone which consent you gave and when. The same version and time are sent with each donation.

Your donor ID does not contain your name. But the video can show who you are, and the upload times, device model and iOS version could be matched against the TestFlight tester list (section 4.5). I commit never to do that matching on purpose, and to use donor IDs only to handle your files and requests. The one exception is when you ask me to find your own files and cannot give me a donor ID (section 9).

### 4.4 Your IP address

Your phone's connection reveals your IP address to Cloudflare, twice: when the app contacts the small upload service (the Worker), and when it sends files to the storage. Cloudflare handles that connection data under its own privacy policy as well as for me (section 6).

The Worker does not store or log your IP address. To keep the service secure and stop abuse (at most 60 requests an hour per address), it keeps a keyed hash of your address (for IPv6, of its first 64 bits) and a request counter. Both are stored in the same storage area, separately from your donations, for about one to two days. The hash is also passed to Cloudflare's burst limiter (20 requests a minute); Cloudflare's documentation does not say how long that limiter keeps it. A hash of this kind is still personal data.

### 4.5 TestFlight data I receive

I invited you through TestFlight, so I see in App Store Connect: your name and the email address on your invitation, which build you installed, and per-tester usage such as sessions and crashes. If you send feedback or a crash report through TestFlight, Apple passes it to me together with your name and email address, your device model, iOS version, app version and build, battery level, carrier, time zone, connection type, free disk space, screen resolution, how long the app had been open and the processor type, plus any comment or screenshot you add. A screenshot can show your own twin or video.

I use this only to run the beta and to answer you and fix the app. Please do not put personal details into feedback you do not want me to have.

### 4.6 Short-lived logs

When you delete your data, the Worker writes one log line with the time, your donor ID and the number of files removed. It contains no content. Cloudflare keeps it for up to 7 days. The Worker's error log lines are kept for the same time. The Worker does not keep a log of every request.

### 4.7 What I do not collect

Contacts, advertising ID, precise location, and the sound of your video. The app contains no analytics, advertising or tracking code from third parties.

### 4.8 Other people in your video

I do not look for other people in the clips and cannot tell who they are. Please film only yourself and keep other people out of the picture. If you appear in someone else's clip, write to me at kinetwin@proton.me and I will look for it and delete it.

## 5. Why I use your data, and the legal basis

| What | Why | Legal basis |
|---|---|---|
| Receiving, storing and using your clip and the files above, including the extras you choose to add | Improve the accuracy of Kinetwin's pose measurement and the app, including testing and training the pose models; research on lifting technique | Your consent, GDPR Art. 6(1)(a): first checkbox |
| The same, for body and fitness data in those files | Same purposes | Your **explicit** consent, Art. 9(2)(a): second checkbox. A video of your body and your lifting measurements may reveal information about your health, so I treat them as special-category data to be safe. |
| Limiting requests per IP address, deletion and error logs | Keep the upload service secure and working; stop abuse | My legitimate interest, Art. 6(1)(f): the service would be open to abuse without it. The data is a hash, kept for a day or two. You can object (section 9). |
| Handling the TestFlight tester list, usage and feedback (4.5) | Run the beta; answer you; fix the app | My legitimate interest, Art. 6(1)(f): I cannot run a beta without knowing who the testers are. You can object (section 9). |

**Joining is the condition of the beta.** The beta exists to collect test data. If you do not agree, do not join: you simply do not take part. Joining is your choice, and consent is the legal basis I rely on for it. Giving me the data is required by no law and no contract; if you do not give it, you cannot take part in the beta. While I hold your data, I keep the record of your consent (version and time) so I can show what you agreed to.

**I use your data only for the purposes above.**
- I do not sell it, rent it or give it to anyone for their own use.
- I do not use it for advertising, profiling or tracking.
- I make no automated decisions about you with legal or similar effect (Art. 22). The app shows you an analysis of your lift; I use the data to improve it.
- Kinetwin is planned as a commercial app and your data helps build it. You are not paid and get no reward for donating.
- Research results are published, if at all, only as aggregate statistics, never as clips or individual pose data.

## 6. Who receives your data

- **Cloudflare, Inc. (USA)**, my processor, for storing your files (R2 storage, EU jurisdiction) and for the small Worker that hands out upload links and deletes data. Cloudflare may act only on my instructions, under its data processing agreement. For its own purposes, such as network security, Cloudflare also handles the connection data (including IP addresses) of visitors to its network. It does that as a separate controller under its privacy policy (https://www.cloudflare.com/privacypolicy/).
- **Apple** runs TestFlight and the tester accounts (section 3 and 4.5). Apple acts under its own privacy policy and passes me the data in 4.5.
- **GitHub** hosts this notice. See section 12.
- **Me, Simon Pastoor.** Nobody else has access to your files. I process them only with tools that run on my own computer. I never send a clip, a frame, `pose.json`, `twin.json`, `velocity.csv` or anything derived from them to an AI service, a cloud-based tool or any other third party. My downloaded copies are kept as described in section 8.
- Authorities, only if the law requires it.

No one else gets your data.

## 7. Where it is stored, transfers outside the EU, and security

Your files are stored in a Cloudflare R2 storage area that is private and has EU jurisdiction. There are no public links. Video goes straight from your phone to that storage over HTTPS. It never passes through the Worker. The Cloudflare account that holds it is protected with two-factor authentication.

The Worker sees the donor ID, the token, the list of files (names, sizes and checksums), the consent version and time, the app version and your IP address, but never the video. It runs on Cloudflare's global network and may be handled outside the EU. The EU guarantee covers where objects are stored, not where the Worker runs. Cloudflare, Inc. is a US company. Transfers to it rest on the EU-US Data Privacy Framework, in which Cloudflare, Inc. is listed, and on the Standard Contractual Clauses that are part of Cloudflare's data processing agreement. You can ask me for a copy of the agreement at kinetwin@proton.me.

Files are encrypted in transit (HTTPS/TLS) and at rest (AES-256, managed by Cloudflare). Upload links work for 15 minutes, for one file each. Read access to the files is limited to me, through a read-only key, and to the upload service (the Worker), which holds a read-and-write key but only checks file sizes and types.

If a data breach puts your rights at high risk, I will tell you through the email address on your TestFlight invitation, and I will report it to the Autoriteit Persoonsgegevens within 72 hours where the law requires it.

## 8. How long I keep it

| What | How long |
|---|---|
| Your donation files, manifests, token hash and counters | About 730 days (24 months) after upload, deleted automatically by a rule in the storage. Deletion can run up to a day late. Earlier, when you delete your data or leave the beta. |
| Donations that were started but not finished | Removed automatically within about 25 hours. |
| IP hash and request counter | About one to two days. |
| Deletion and error log lines | Up to 7 days, at Cloudflare. |
| Copy on your phone | Until it is uploaded. A copy that is waiting is removed when you delete your data or leave the beta. |
| My working copies of your files | Kept only on one encrypted volume on my computer that is excluded from cloud sync and backups. Before each use I compare it with the storage and delete anything that is no longer there. Everything is gone at 730 days at the latest. |
| TestFlight feedback and crash reports | Deleted once answered, and at the latest 12 months after I receive them. |
| TestFlight tester list (name and email) | While you are a tester. I remove you when you email me that you are leaving, or when the beta ends. Leaving in the app does not tell me. You can also stop testing yourself in the TestFlight app. |
| Cloudflare's own connection data | Under Cloudflare's own privacy policy. |
| Trained or tuned models | See below. |

**Models.** A model trained or tuned with your data is not retrained on request. It is not meant to contain your clip, but it cannot unlearn it. I build each training set from the files that exist in the storage at that time, so deleted data drops out of all later training.

## 9. Your rights and how to use them

I answer within one month (Art. 12(3)). If your request is complicated I may extend that by up to two further months, and I will tell you why within the first month. Requests are free.

| Right | How |
|---|---|
| Delete your data (Art. 17) | In the app: **Beta settings > Delete my data**. It removes everything stored under your donor ID and gives you a new random ID. **You stay in the beta, and later clips are uploaded again.** To stop uploads, use Leave the beta. |
| Withdraw consent (Art. 7(3)) | In the app: **Beta settings > Leave the beta**. It withdraws both consents on the spot, stops uploads, removes clips still waiting on your phone, locks the app and then deletes your data. If you are offline when you tap it, the consent is still withdrawn and the app retries the deletion each time you open it until the server confirms. **Keep Kinetwin installed until the deletion screen disappears;** if you delete the app first, the retry is lost. Leaving in the app does not tell me and does not remove you from TestFlight: email me, or stop testing in the TestFlight app. Processing before withdrawal stays lawful. |
| Access and a copy (Arts. 15, 20) | Email kinetwin@proton.me. There is no in-app export, so I prepare the copy by hand. Give me your donor ID, which the app shows in Beta settings. |
| Correct, restrict or object (Arts. 16, 18, 21) | Email kinetwin@proton.me. An upload cannot be edited: delete it and, if you wish, donate again. You may object to the IP-address rate limiting and to the tester-list processing. |
| Complain | To the Autoriteit Persoonsgegevens (https://autoriteitpersoonsgegevens.nl), or to the authority where you live or work. You are welcome to tell me first. |

**How I check that a request is yours.** A donor ID is not a secret. So, for access requests and for requests by email, send me the donor ID plus two things only the owner would know, for example your device model and the approximate date and length of one clip. I match them against the files. I send the copy as an encrypted download link to the address you wrote from, and give you the password separately.

**If the app cannot delete for you** (for example you lost the donor ID or the app's secret token, or got a new phone), email me. Tell me your device model, the dates of your uploads and what the clips show, and I will try to find and delete them. I cannot promise to find them without your donor ID. Whatever is left is deleted after about 730 days.

**If you delete the app without using Delete my data,** your files stay until the 730 days are over. On the same iPhone, iOS can keep your donor ID and token in the Keychain after the app is deleted, so a reinstall may recover them, but that is not guaranteed. Delete first.

**Uploads that were on their way when you deleted** can arrive late. A cleaning job removes them within about two hours. In rare cases a leftover hash of your old token can stay until the 730 days are over; it holds no content and no name.

## 10. Age and language

The beta is for adults only (18 or older). The consent screen asks you to confirm it. I do not check it any further. If you are under 18, please do not join.

The beta is in English only. Join only if you read English comfortably.

## 11. Changes

If I ever collect a new kind of data, use the data for a new purpose, or share it with anyone new, I will publish a new notice and ask for your consent again (`kinetwin-beta-consent-3` or higher) before anything changes. The app stays locked until you answer. For changes that do not affect what you agreed to, I publish a new version of this notice and change the date at the top.

## 12. This website

This notice is hosted on GitHub Pages. GitHub logs the IP address of every visitor to a Pages site for security purposes, under GitHub's own privacy statement (https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). I do not add analytics or cookies to the page.

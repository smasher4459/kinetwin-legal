---
layout: default
title: Kinetwin beta privacy notice
description: Privacy notice for the Kinetwin TestFlight beta (version beta-notice-v4).
permalink: /privacy/
---

# Kinetwin beta: privacy notice

Version `beta-notice-v4` · 4 November 2026 · applies to consent version `kinetwin-beta-consent-3` and to the consent email `kinetwin-participant-consent-2` · covers the Kinetwin TestFlight beta only, including people I filmed on my phone for it

Published at https://smasher4459.github.io/kinetwin-legal/privacy/

Earlier versions stay available at the same address. In this notice "I" and "me" mean Simon Pastoor, the person responsible for your data. "Kinetwin" means the iPhone app.

## 1. The short version

- **Donating is optional.** Kinetwin works fully without it. If you choose to donate, you turn donating on once and then confirm each clip before it is uploaded. If you say no, nothing is uploaded and you lose nothing.
- Separately, because I invited you through TestFlight, I see your name, email address and any feedback you send, whether or not you donate (section 4.5).
- **If I filmed you on my phone** and you do not use the app, section 3 says which parts of this notice apply to you.
- What goes up, only for a clip you donate: your video (with the sound and the hidden information inside the video file removed), the body pose, 3D twin and measurements Kinetwin made from it, and some technical details about your phone and the video. If you add them, also your known 1RM, the weight of a set and a bar-velocity file.
- Your video can show your face and body. Anything stored under a random donor ID can still be about you, so it is **pseudonymised, not anonymous**.
- Only I can use it, unless you agree in writing to more (two points down). I use it to improve Kinetwin and for research on lifting technique. I do not sell it, I do not show you ads, and the app contains no advertising or tracking code.
- Files are stored in a private storage area in the EU at Cloudflare, my service provider. They are deleted automatically after about 730 days (24 months), or earlier when you delete them in the app. The reason for 730 days is in section 8.
- **Google Drive and AI services, only if you agree in writing.** I may ask you by email whether I may keep your data in my personal Google Drive and send it to Google Antigravity, Anthropic Claude, or OpenAI ChatGPT and Codex. You answer YES or NO for each service separately; a service you do not answer YES is a no. I do this only for the services you answered YES. These are consumer services on my personal accounts: each company handles what I send as its own controller, and its staff may look at it. Copies kept this way have no fixed end date, but I ask you each year to confirm, and I stop sending data to these consumer AI services when Kinetwin is released to the public. If you do not reply YES, nothing changes: your data stays as this notice describes, and no AI service receives it. Details in sections 5 to 9.
- You can stop donating, delete your data or leave the beta at any time in **Beta settings** (**Stop donating**, **Delete my data**, **Leave the beta**).

## 2. Who is responsible

| | |
|---|---|
| Controller | Simon Pastoor, an individual developer in the Netherlands |
| Contact for anything in this notice | kinetwin@proton.me (you may write in English or Dutch) |
| Data protection officer | None. Not required at this scale (GDPR Art. 37). |
| Supervisory authority | Autoriteit Persoonsgegevens (AP), the Dutch data protection authority |

## 3. What this notice covers

This notice covers the data the Kinetwin beta uploads when you choose to donate a clip, and the other data I handle to run the beta, including for testers who never donate (section 4.5), and the videos of people I filmed on my phone (end of this section). It does not cover:

- **Apple and TestFlight.** Apple runs TestFlight. Apple handles your invitation, your installs and its own crash and usage reports under Apple's own privacy policy (https://www.apple.com/legal/privacy/). Section 4.5 says what Apple passes on to me.
- **A later public Kinetwin app.** It will have its own notice and its own consent.

Your analysis runs on your phone. Nothing is uploaded until you tick both boxes, tap **Turn on donating**, and then confirm the clip with **Donate this clip**.

**People I filmed on my phone.** Some people take part without the app: I film their lifts on my own phone. If that is you, I keep the videos and what my software makes from them: body pose and joint positions, a 3D model of your body, your height and measurements of your lifts. Before I use the videos further, I ask for your permission in writing by email (`kinetwin-participant-consent-2`). Until you reply, I keep the videos in my Google Drive and do nothing else with them. If you say no, I delete them within 30 days. If you say yes, sections 5 to 9 apply to you as they apply to Google Drive and the AI services. Sections 4.1 to 4.6 (the app, the donor ID, the Cloudflare storage and TestFlight) do not apply to you. I label your data with a participant code, not your name, before it goes anywhere. Before a video goes to an AI service, I remove its sound and location data, and I crop or blur anyone else who can be recognised in it.

## 4. What I collect

### 4.1 The files of each donation

When you tap **Donate this clip**, the app starts uploading these files right away. The video goes over Wi-Fi only, not over mobile data or a personal hotspot; the smaller files can use any connection. If the upload does not finish before Kinetwin closes, the files wait on your phone. The app does not send them by itself the next time you open it: it shows how many donations are waiting and sends them only when you tap **Send**. They are the only file names the server accepts.

| File | What it is |
|---|---|
| `clip.mov` or `clip.mp4` | Your video of the lift, up to 600 MB. The app removes the sound and the information stored inside the video file (such as GPS location, device make and model, software and recording date) before it uploads. The picture itself is not changed: it may show your face, your body, the room and other people near you. |
| `pose.json` | The 3D body pose the app measured in each frame (joint positions). |
| `twin.json` | The script of your 3D twin, the animated skeleton the app builds from your lift. |
| `metrics.json` | Two measurements calculated from the twin: bar vertical travel and the largest sideways offset of the bar, each with a note on how uncertain it is. |
| `meta.json` | Technical details, listed in 4.2. |
| `feedback.json` (optional) | Two numbers, only if you fill them in: your known one-repetition maximum and the weight of the set, in kilograms. No free text. |
| `velocity.csv` (optional) | A file you choose from the Files app, exported from a bar-velocity sensor. It is sent exactly as it is, without being read or changed. Remove names and other personal details from it before you choose it. |
| `velocity_meta.json` (optional) | The sensor brand you pick, the export date you pick and the number of rows in the file. |

### 4.2 What `meta.json` holds

- app version and build;
- device model;
- iOS version;
- region only (for example NL), not your full language setting;
- where the clip came from in the app (Photos or Files). Kinetwin imports videos that are already on your iPhone; it does not record video, so it has no camera or microphone access;
- video format: codec, size, frame rate, duration and rotation;
- the camera lens name (which can include your phone model) and its focal length, if your video file records them (never location or date);
- the height you typed, and where it came from;
- the Vision request revision and, per refusal reason, how many frames the pose analysis refused;
- the analysis time;
- the consent version;
- the time you confirmed this clip with **Donate this clip**.

### 4.3 Identifiers and records

- **Donor ID and token.** On first launch the app makes a random donor ID and keeps a random secret token in your iPhone Keychain. Your files are stored under the donor ID. The server keeps only a SHA-256 hash of the token, so that only your phone can order deletion.
- **A manifest for every donation** (`_manifest.json`). It lists the donor ID, a donation ID, when the donation was started and completed, the app version, the consent version and the time you consented, and, for each file, its name, size and checksum.
- **Counters.** A daily counter of how many donations your donor ID started, and markers for donations that have been started but not finished.
- **Consent record.** The app stores on your phone which consent you gave and when. The same version and time are sent with each donation, together with the time you confirmed that clip.

Your donor ID does not contain your name. But the video can show who you are, and the upload times, device model and iOS version could be matched against the TestFlight tester list (section 4.5). I commit never to do that matching on purpose, and to use donor IDs only to handle your files and requests. There are two exceptions: when you ask me to find your own files and cannot give me a donor ID (section 9), and when you agree in writing to Google Drive or an AI service (section 6), because I then need to know which files are yours. For that, the consent email asks you to put your donor ID in your reply.

### 4.4 Your IP address

Your phone's connection reveals your IP address to Cloudflare, twice: when the app contacts the small upload service (the Worker), and when it sends files to the storage. Cloudflare handles that connection data under its own privacy policy as well as for me (section 6).

The Worker does not log or store your IP address. To keep the service secure and stop abuse (at most 60 requests an hour per address), it turns your address (for IPv6, its first 64 bits) into a keyed one-way hash: HMAC-SHA256 with a secret salt kept in the Worker's secrets, cut to 128 bits. It counts requests per hash. The counter is stored in the same storage area, separately from your donations, and is deleted after about a day. The hash is also passed to Cloudflare's burst limiter (20 requests a minute); Cloudflare's documentation does not say how long that limiter keeps it. A hash of this kind is still personal data. Cloudflare's network itself handles your address to route the request (section 6).

### 4.5 TestFlight data I receive

This section applies to every tester, whether or not you donate. I invited you through TestFlight, so I see in App Store Connect: your name and the email address on your invitation, which build you installed, and per-tester usage such as sessions and crashes. If you send feedback or a crash report through TestFlight, Apple passes it to me together with your name and email address, your device model, iOS version, app version and build, battery level, carrier, time zone, connection type, free disk space, screen resolution, how long the app had been open and the processor type, plus any comment or screenshot you add. A screenshot can show your own twin or video.

I use this only to run the beta and to answer you and fix the app. Please do not put personal details into feedback you do not want me to have.

### 4.6 Short-lived logs

When you delete your data, the Worker writes one log line with the time, your donor ID and the number of files removed. It contains no content. Cloudflare keeps it for up to 7 days. The Worker's error log lines are kept for the same time. The Worker does not keep a log of every request.

### 4.7 What I do not collect

Contacts, advertising ID, precise location, and the sound of your video. The app contains no analytics, advertising or tracking code from third parties.

### 4.8 Other people in your video

I do not look for other people in the clips and cannot tell who they are. Please film only yourself and keep other people out of the picture. If you appear in someone else's clip, write to me at kinetwin@proton.me and I will look for it and delete it. If a person who donated agreed in writing to the AI services (section 6), I crop or blur anyone else who can be recognised in a video before it goes to an AI service.

## 5. Why I use your data, and the legal basis

| What | Why | Legal basis |
|---|---|---|
| Receiving, storing and using the clips you donate and the files above, including the extras you choose to add | Improve the accuracy of Kinetwin's pose measurement and the app, including testing and training the pose models; research on lifting technique | Your consent, GDPR Art. 6(1)(a): first checkbox, and your confirmation of each clip |
| The same, for body and fitness data in those files | Same purposes | Your **explicit** consent, Art. 9(2)(a): second checkbox. A video of your body and your lifting measurements may reveal information about your health, so I treat them as special-category data to be safe. |
| Keeping your data in my Google Drive, and on my computer while analysis runs, if you replied YES to Box A of my consent email. For people I filmed on my phone, this is all my use of the videos. | Develop and test Kinetwin's analysis and models | Your **explicit** consent, Art. 6(1)(a) and 9(2)(a): your written YES to Box A |
| Sending your data to the AI services you marked YES (the services you answered YES in Box B of the consent email; section 6) | Develop and test Kinetwin's analysis and models: check and improve the analysis and write the code | Your **explicit** consent, Art. 6(1)(a) and 9(2)(a): your written YES to each box. |
| Keeping the videos I filmed on my phone in my Google Drive until you answer my consent email, without using them | Ask you before I use them, and delete them if you say no | My legitimate interest, Art. 6(1)(f), in asking you before deciding. You can object (section 9); I then delete them. |
| Keeping the record of your consent (version and time in the app; your email reply) | Show what you agreed to (Art. 7(1)) | Legal obligation, Art. 6(1)(c) |
| Limiting requests per IP address, deletion and error logs | Keep the upload service secure and working; stop abuse | My legitimate interest, Art. 6(1)(f): the service would be open to abuse without it. The data is a keyed hash, kept for about a day. You can object (section 9). |
| Handling the TestFlight tester list, usage and feedback (4.5) | Run the beta; answer you; fix the app | My legitimate interest, Art. 6(1)(f): I cannot run a beta without knowing who the testers are. You can object (section 9). |

**Donating is optional.** Kinetwin works fully without it, and saying no changes nothing about what you can do in the app. Donating is a separate choice, and consent is the legal basis I rely on for it. Giving me the data is required by no law and no contract, and you lose nothing by not giving it. The same goes for the consent email: every box is optional, anything you do not mark YES counts as NO, and saying no changes nothing about your place in testing. You can withdraw your consent at any time, as easily as you gave it (section 9). While I hold your data, I keep the record of your consent (version and time, and your email reply if you sent one) so I can show what you agreed to.

**I use your data only for the purposes above.**
- I do not sell it or rent it. I give it to nobody for their own use, except the services you agree to in writing: each handles what I send as its own controller (section 6).
- I do not use it for advertising, profiling or tracking.
- I make no automated decisions about you with legal or similar effect (Art. 22). The app shows you an analysis of your lift; I use the data to improve it.
- Kinetwin is planned as a commercial app and your data helps build it. You are not paid and get no reward for donating.
- Research results are published, if at all, only as aggregate statistics, never as clips or individual pose data.

## 6. Who receives your data

- **Cloudflare, Inc. (USA)**, my processor, for storing your files (R2 storage, EU jurisdiction) and for the small Worker that hands out upload links and deletes data. Cloudflare may act only on my instructions, under its data processing agreement. For its own purposes, such as network security, Cloudflare also handles the connection data (including IP addresses) of visitors to its network. It does that as a separate controller under its privacy policy (https://www.cloudflare.com/privacypolicy/).
- **Apple** runs TestFlight and the tester accounts (section 3 and 4.5). Apple acts under its own privacy policy and passes me the data in 4.5.
- **GitHub** hosts this notice. See section 12.
- **Me, Simon Pastoor.** I give nobody else access to your files, except as in the next point. (Under its agreement with me, Cloudflare must let only its authorised staff reach stored data.) Unless you agreed in writing (next point), I process the files only with tools that run on my own computer, and I never send a clip, a frame, `pose.json`, `twin.json`, `velocity.csv` or anything derived from them to an AI service, a cloud-based tool or any other third party. My downloaded copies are kept as described in section 8.
- **Google Drive and three AI services, only if you agreed in writing, for each service.** If you replied YES to my consent email (`kinetwin-participant-consent-2`), I keep your data in my personal Google Drive, in a folder only I can open, and on my own computer while analysis runs. I send it only to the AI services you marked YES, to check and improve the analysis and write the code. Anything you did not mark YES counts as NO.
  - **Google Drive** and **Google Antigravity**: Google Ireland Limited. In Antigravity, training is switched off (setting "telemetry"). Google still uses what I send to run the service and keep it safe. In Antigravity I use only Google's Gemini models for your data, unless you also marked YES for Anthropic.
  - **Anthropic Claude** (including Claude Code): Anthropic Ireland, Limited. Training switched off ("Help improve Claude").
  - **OpenAI ChatGPT and Codex**: OpenAI Ireland Limited. Training switched off ("Improve the model for everyone").

  The three AI services are consumer services on my personal accounts. That means: each company handles what I send under its own terms and privacy policy, as its own controller; there is no contract between the company and me about your data; and its staff may look at it, for example for safety checks. Before sending anything I switch off, wherever the service offers it, the setting that lets the company train its AI on my chats. Google Drive is also on my personal account: it is Google's consumer service, and Google stores the files under its own terms and privacy policy. I label your data with a participant code, not your name, before it goes anywhere. Before a video goes to an AI service, I remove its sound and location data and crop or blur anyone else who can be recognised in it. Where each company processes your data: section 7. How long it keeps it: section 8.
- Authorities, only if the law requires it.

Nobody else receives your data for their own use, except that Cloudflare handles connection data such as IP addresses for its own network security, and the services you agreed to in writing handle what I send as their own controllers (both above).

## 7. Where it is stored, transfers outside the EU, and security

Your files are stored in a Cloudflare R2 storage area that is private and has EU jurisdiction. There are no public links. Video goes straight from your phone to that storage over HTTPS. It never passes through the Worker. The Cloudflare account that holds it is protected with two-factor authentication.

The Worker sees the donor ID, the token, the list of files (names, sizes and checksums), the consent version and time, the app version and your IP address, but never the video. It runs on Cloudflare's global network and may be handled outside the EU. The EU guarantee covers where objects are stored, not where the Worker runs. Cloudflare, Inc. is a US company. Transfers to it rest on the EU-US Data Privacy Framework, in which Cloudflare, Inc. is listed, and on the Standard Contractual Clauses that are part of Cloudflare's data processing agreement. You can ask me for a copy of the agreement at kinetwin@proton.me.

**Google Drive and the AI services (only if you agreed in writing).** Google Ireland Limited, Anthropic Ireland, Limited and OpenAI Ireland Limited are in Ireland, in the EU. Anthropic, OpenAI and Google may also process data in the USA under their own safeguards. Your data is not sent to any other AI service, and in particular not to any service that stores data in China.

Files are encrypted in transit (HTTPS/TLS) and at rest (AES-256, managed by Cloudflare). Upload links work for 15 minutes, for one file each. Read access to the files is limited to me, through a read-only key, and to the upload service (the Worker), which holds a read-and-write key but only checks file sizes and types.

If a data breach puts your rights at high risk, I will tell you through the email address on your TestFlight invitation (if I filmed you on my phone: the address you replied from), and I will report it to the Autoriteit Persoonsgegevens within 72 hours of becoming aware of it where the law requires it.

## 8. How long I keep it

| What | How long |
|---|---|
| Your donation files, manifests, token hash and counters | About 730 days (24 months) after upload, deleted automatically by a rule in the storage. Deletion can run up to a day late. Earlier, when you delete your data or leave the beta. |
| Donations that were started but not finished | Removed automatically within about 25 hours. |
| IP hash and request counter | About one day. |
| Deletion and error log lines | Up to 7 days, at Cloudflare. |
| Copy on your phone | Until it is uploaded. Every copy that is waiting is removed when you stop donating, delete your data or leave the beta. The folder that holds them is excluded from iCloud Backup. If you choose Don't donate this clip, nothing is written for upload. The working copy Kinetwin makes for the analysis is deleted when you tap Start over and each time the app starts. Your original video in Photos or Files is never touched. |
| My working copies of your files | Kept only on one encrypted volume on my computer that is excluded from cloud sync and backups. Before each use I compare it with the storage and delete anything that is no longer there. Everything is gone at 730 days at the latest. If you agreed in writing to Google Drive, the next row applies to your copies instead. |
| Copies in my Google Drive, on my computer and in chats with the AI services, only if you agreed in writing | No fixed end date. I keep your data for as long as I develop Kinetwin's analysis and models with it, and delete it when you ask me to or when I stop developing Kinetwin, whichever comes first. Each year I check whether I still need it, and delete it if I do not. When I delete it, I also delete the chats that contain it and ask each company to delete what I sent. Your files in the Cloudflare storage still follow the first row. |
| What each AI company keeps | Google Antigravity keeps it until I ask Google to delete it. Anthropic: chats I delete are removed within 30 days; chats flagged by Anthropic's safety systems can be kept for up to 2 years and used even with training off. OpenAI: chats I delete are removed within 30 days, longer if OpenAI must keep them for safety or legal reasons. Google Drive: files I delete are removed by Google under its own terms and privacy policy. |
| Videos I filmed on my phone, before you reply | Kept in my Google Drive, unused, until you reply. |
| Videos I filmed on my phone, if you say no | Deleted within 30 days. |
| TestFlight feedback and crash reports | Deleted once answered, and at the latest 12 months after I receive them. |
| TestFlight tester list (name and email) | While you are a tester. I remove you when you email me that you are leaving, or when the beta ends. Leaving in the app does not tell me. You can also stop testing yourself in the TestFlight app. |
| Cloudflare's own connection data | Under Cloudflare's own privacy policy. |
| Trained or tuned models | See below. |

**Why 730 days.** The law sets no number of days for this (GDPR Art. 5(1)(e)); 730 days is my own judgement. The reason: developing Kinetwin's models and checking them across app versions needs comparison data over about two years. 730 days is a maximum, not a target. The beta may end earlier, and you can delete your data at any time.

**Models.** A model trained or tuned with your data is not retrained on request. It is not meant to contain your clip, but it cannot unlearn it. I build each training set from the files that exist in the storage at that time, so deleted data drops out of all later training. No model is trained on donated clips until a written model assessment exists; if it finds that a model could keep your personal data, I ask for new consent before any training. This is about my own models. Separately, if you marked YES for it: Anthropic can use chats its safety systems flag even with training off (section 6). I cannot undo that.

## 9. Your rights and how to use them

I answer within one month (Art. 12(3)). If your request is complicated I may extend that by up to two further months, and I will tell you why within the first month. Requests are free.

| Right | How |
|---|---|
| Delete your data (Art. 17) | If you agreed in writing to Google Drive or an AI service, or I filmed you on my phone, email kinetwin@proton.me: I then delete your copies in Google Drive and on my computer and the chats that contain your data, and ask each company to delete what I sent. In the app: **Beta settings > Delete my data**. It asks the server to delete everything stored under your donor ID, removes clips still waiting on your phone and then gives you a new random ID. **It also turns donating off:** to donate again, you tick both boxes again. Until the server confirms the deletion, Beta settings says your earlier data is still being deleted, you cannot turn donating on, and the app retries each time you open it (or when you tap **Retry deletion**). If the server refuses, the app asks you to email me. |
| Withdraw consent (Art. 7(3)) | In the app: **Beta settings > Leave the beta**. It withdraws both consents on the spot, stops uploads, removes clips still waiting on your phone and then deletes your data. Kinetwin stays usable afterwards. To stop donating without deleting what you already gave, tap **Beta settings > Stop donating**: it stops uploads and removes clips still waiting on your phone, but keeps what you already uploaded and does not withdraw your consent for those clips. To donate again after either, you tick both boxes again. If you are offline when you tap Leave the beta, the consent is still withdrawn and the app retries the deletion each time you open it until the server confirms. **Keep Kinetwin installed until Beta settings no longer says that your earlier data is still being deleted;** if you delete the app first, the retry is lost. Leaving in the app does not tell me and does not remove you from TestFlight: email me, or stop testing in the TestFlight app. Processing before withdrawal stays lawful. |
| Withdraw consent for Google Drive or an AI service | Email kinetwin@proton.me, or reply to my consent email. You can withdraw any box on its own. From then on I send nothing more to that service, and within 30 days I delete the chats that contain your data and ask the company to delete what it kept. **Leave the beta and Delete my data in the app do not reach Google Drive or the AI services, because the app does not tell me: email me as well.** Withdrawing does not undo what happened before. |
| Access and a copy (Arts. 15, 20) | Email kinetwin@proton.me. There is no in-app export, so I prepare the copy by hand. Give me your donor ID, which the app shows in Beta settings. |
| Correct, restrict or object (Arts. 16, 18, 21) | Email kinetwin@proton.me. An upload cannot be edited: delete it and, if you wish, donate again. You may object to the IP-address rate limiting, to the tester-list processing and, if I filmed you on my phone, to my keeping the videos until you reply. |
| Complain | To the Autoriteit Persoonsgegevens (https://autoriteitpersoonsgegevens.nl), or to the authority where you live or work. You are welcome to tell me first. |

**How I check that a request is yours.** A donor ID is not a secret. So, for access requests and for requests by email, send me the donor ID plus two things only the owner would know, for example your device model and the approximate date and length of one clip. I match them against the files. If I filmed you on my phone, write from the address you used for the consent email instead. I send the copy as an encrypted download link to the address you wrote from, and give you the password separately.

**If the app cannot delete for you** (for example you lost the donor ID or the app's secret token, or got a new phone), email me. Tell me your device model, the dates of your uploads and what the clips show, and I will try to find and delete them. I cannot promise to find them without your donor ID. Whatever is left is deleted after about 730 days.

**After your TestFlight build expires.** A TestFlight build can be tested for at most 90 days, and then it no longer opens, so Beta settings cannot be reached. Your files can stay for up to 730 days. Email kinetwin@proton.me for any right in this section; I will ask for your donor ID, or for the facts above if you no longer have it.

**If you delete the app without using Delete my data,** your files stay until the 730 days are over. On the same iPhone, iOS can keep your donor ID and token in the Keychain after the app is deleted, so a reinstall may recover them, but that is not guaranteed. Delete first.

**Uploads that were on their way when you deleted** can arrive late. A cleaning job removes them within about two hours. In rare cases a leftover hash of your old token can stay until the 730 days are over; it holds no content and no name.

## 10. Age and language

The beta is for adults only (18 or older). The consent screen and the consent email ask you to confirm it. I do not check it any further. If you are under 18, please do not join.

The beta is in English only. Join only if you read English comfortably.

## 11. Changes

If I ever collect a new kind of data, use the data for a new purpose, or share it with anyone new, I will publish a new notice and ask for your consent again (`kinetwin-beta-consent-4` or higher) before anything changes. Donating stays off until you answer. Version 4 of this notice is such a change: it adds Google Drive and three AI services. I ask for that consent by email (`kinetwin-participant-consent-2`), one box per service, not in the app. Only people who reply YES are affected. For changes that do not affect what you agreed to, I publish a new version of this notice and change the date at the top.

## 12. This website

This notice is hosted on GitHub Pages. GitHub logs the IP address of every visitor to a Pages site for security purposes, under GitHub's own privacy statement (https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement). I do not add analytics or cookies to the page.

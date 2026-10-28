---
layout: default
title: Kinetwin beta participant information
description: Participant information for the Kinetwin TestFlight beta (version beta-sheet-v2).
permalink: /beta/
---

# Kinetwin beta: participant information

Version `beta-sheet-v2` · dated 28 October 2026 · consent version `kinetwin-beta-consent-2` · for invited adults (18+)

Please read this before you install the build. The full privacy notice is at https://smasher4459.github.io/kinetwin-legal/. In this sheet "I" means Simon Pastoor, the person responsible for your data.

## What this beta is

Kinetwin turns a video of your lift into a 3D "twin". This TestFlight beta exists to collect test data so I can make Kinetwin more accurate. **Joining means every clip you analyse is uploaded.** If you do not want that, do not join. You lose nothing by saying no.

The beta is in English only. Join only if you read English comfortably.

## What is uploaded

When you finish with a clip (when you tap **Start over**, or the next time you open the app), the app uploads:

- your **video clip**. The app removes the sound and the information hidden in the video file (such as GPS location, device and recording date) first. The picture can still show your face, body and surroundings;
- the **pose**, **twin** and **metrics** files the app produced from it;
- **technical details** (`meta.json`): app, device and iOS version, region only, where the clip came from (Photos or Files), the video format, the height you typed, analysis details and the consent version (full list in the notice);
- **only if you add them:** a bar-velocity file from your sensor (sent as it is, so remove names and personal details from it first), your known 1RM and the weight of a set.

Not collected: your contacts, advertising ID or precise location. Your files are stored under a random donor ID, not your name. That is pseudonymised, not anonymous: the video can show who you are.

Until a clip is uploaded, a copy of it waits on your phone. Video files upload over Wi-Fi only. Expect large uploads, up to 600 MB per clip.

## Who sees it, where, for how long

Only I do. The files sit in private storage in the EU at Cloudflare, my service provider, and are deleted automatically after about 730 days (24 months). I use them to improve Kinetwin's pose accuracy and the app, including training and testing models, and for research on lifting technique. They are not sold, shared or used for advertising. I never send a clip or analysis file to an AI service or any other third party. You are not paid for taking part.

Apple runs TestFlight. Through it I also see your name and email address, your usage and any feedback you send (section 4.5 of the notice).

## Your choices, any time, in Beta settings

- **Delete my data**: removes everything stored under your donor ID and gives you a new random ID. **You stay in the beta and later clips are uploaded again.**
- **Leave the beta**: withdraws your consent at once, stops uploads, locks the app and deletes your data. If you are offline, the consent is still withdrawn and the app retries the deletion each time you open it.
- **Your donor ID** is shown in Beta settings. Keep it if you want to ask me for a copy of your data.
- You can also email kinetwin@proton.me, or complain to the Autoriteit Persoonsgegevens (https://autoriteitpersoonsgegevens.nl).

A model already trained or tuned with your data is not retrained when you delete (notice, section 8); data you delete drops out of all later training.

Delete before you uninstall. If you delete the app without deleting your data, your files stay until they expire after about 730 days, and I may not be able to tell which are yours.

## Please

- Film only yourself. Keep other people out of the picture.
- Remember the clip can identify you. Do not join if that is a problem for you.
- Do not put personal details into feedback, screenshots or the velocity file that you do not want me to have.

## The consent screen

The first-launch screen blocks the app until you choose. These are the exact texts, fixed under `kinetwin-beta-consent-2`. Any change to the wording, the files collected or the purposes means a new version and fresh consent.

**Summary shown above the boxes**

> Kinetwin is in a test phase. The beta works only for testers who donate their data.
>
> If you join, every clip you analyse is uploaded to private storage in the EU. The sound and the information hidden in the video file, such as location, are removed first. With the clip go what Kinetwin makes from it (body pose, 3D twin and measurements) and technical details: your device model, iOS version, app version, region, the height you type and details about the video. If you add them, your known 1RM, set load and bar-velocity file are uploaded too.
>
> Simon Pastoor is responsible for your data. He uses it only to improve Kinetwin's pose accuracy and the app, and for research on lifting technique. It is not sold and not used for advertising. It is stored under a random ID, not your name, but your video can show who you are. It is deleted automatically after about 24 months (730 days). In Beta settings you can delete your data or leave the beta at any time.

("Read the full privacy notice" links to https://smasher4459.github.io/kinetwin-legal/.)

**Checkbox 1: participation and upload** (unticked by default)

> I am 18 or older and I want to join the Kinetwin beta. I agree that every clip I analyse, with its analysis files, any extras I add and my device details, is uploaded to Kinetwin's private EU storage, so that Simon Pastoor can use it to improve Kinetwin's pose accuracy and the app, and for research on lifting technique.

**Checkbox 2: explicit consent for body and fitness data** (unticked by default)

> I give my explicit consent to Simon Pastoor processing my body and fitness data for those purposes: my video, my body pose and joint positions, my height, my lifting measurements, and my 1RM, set load and bar-velocity file if I add them. I understand this may reveal information about my body and health. I can withdraw this consent at any time with Leave the beta, and that does not affect what happened before.

**Buttons**

- **Join the beta**: enabled only when both boxes are ticked.
- **Don't join**: nothing is uploaded. iOS does not let an app close itself, so Kinetwin shows a locked screen where you can read the terms again or delete the app.

**Stored on the phone and sent with each donation:** `consentVersion = "kinetwin-beta-consent-2"` and `consentedAt` (ISO 8601, UTC) of the moment Join the beta was tapped.

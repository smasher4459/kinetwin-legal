---
layout: default
title: Kinetwin beta participant information
description: Participant information for the Kinetwin TestFlight beta (version beta-sheet-v5).
permalink: /beta/
---

# Kinetwin beta: participant information

Version `beta-sheet-v5` · 5 November 2026 · matches privacy notice `beta-notice-v5` of 5 November 2026 · consent versions `kinetwin-beta-consent-3` (the consent screen in the app), `kinetwin-participant-consent-2` (my consent email) and `kinetwin-beta-cloud-training-addon-2` (my cloud and training email) · for invited adults (18+)

Published at https://smasher4459.github.io/kinetwin-legal/beta/

Please read this before you install the build. The full privacy notice is at https://smasher4459.github.io/kinetwin-legal/privacy/. "Section" below means a section of that notice. In this sheet "I" means Simon Pastoor, the person responsible for your data.

If I filmed you on my phone and you do not use the app, this sheet is not about you: section 3 of the notice says what applies to you.

## What this beta is

Kinetwin turns a video of your lift into a 3D "twin". This TestFlight beta lets you try it. **You can use Kinetwin fully without donating anything.** If you want to help, you can choose to donate clips so I can make Kinetwin more accurate. Donating is a separate choice, and you confirm each clip before it is uploaded. If you say no, nothing is uploaded and you lose nothing.

The beta is in English only. Join only if you read English comfortably.

## Risk and benefit

- **Risk:** the video can show your face and body, so a donated clip can identify you even without your name, and a model trained with your data (only if you agree to training by email) may keep traces of it. If you also agree in writing to the AI services (below), the companies you choose receive your data under their own terms.
- **Benefit:** none for you. You are not paid and get no reward, and Kinetwin works fully without donating. It helps me improve Kinetwin, which is planned as a commercial app.

## What is uploaded

Only for a clip you confirm with **Donate this clip**. The app starts the upload right away (section 4.1). It sends:

- your **video clip**. The app first removes the sound and the information stored inside the video file (such as GPS location, device make and model, software and recording date). The picture itself is not changed: it can show your face, your body, the room and other people near you;
- the **pose**, **twin** and **metrics** files the app produced from it;
- **technical details** (`meta.json`): app version, device model and iOS version, region only, where the clip came from (Photos or Files; Kinetwin imports existing videos and does not record), the video format, the camera lens name and focal length if your video file records them, the height you typed, analysis details, the consent version and the time you confirmed the clip (full list in section 4.2);
- **only if you add them:** a bar-velocity file from your sensor (sent as it is, so remove names and personal details from it first) with the sensor brand, export date and number of rows, your known 1RM and the weight of a set.

Not collected: your contacts, advertising ID, precise location or the sound of your video. The app contains no analytics, advertising or tracking code from third parties (section 4.7). Your files are stored under a random donor ID, not your name. That is pseudonymised, not anonymous: the video can show who you are.

The video uploads over Wi-Fi only, not over mobile data or a personal hotspot. The smaller files can use any connection. Expect large uploads, up to 600 MB per clip. If the upload does not finish before Kinetwin closes, the files wait on your phone, in a folder excluded from iCloud Backup. The app does not send them by itself the next time you open it: it shows how many donations are waiting and sends them only when you tap **Send**. If you choose **Don't donate this clip**, nothing is written for upload (sections 4.1, 8).

## Who sees it, where, for how long

Unless you agree in writing to more (next section), only I use your files. They sit in private storage in the EU at Cloudflare, my service provider. Under its agreement with me, Cloudflare must let only its authorised staff reach stored data (section 6). Cloudflare also sees your IP address when the app connects. The upload service keeps only a scrambled code of it, for about a day, to stop abuse (section 4.4).

The files are deleted automatically after about 730 days (24 months) at the latest, or earlier when you delete them in the app. 730 days is my own judgement: developing Kinetwin's models and checking them across app versions needs comparison data over about two years. It is a maximum, not a target (section 8).

I use them to improve Kinetwin's pose accuracy and the app, including testing models, and for research on lifting technique. I train models on your clips only if you agree by email (below). I do not sell them or use them for advertising. I give them to nobody for their own use, except the services you agree to in writing (section 5). Unless you agree in writing, I process them only with tools that run on my own computer, and I never send a clip, a frame or anything made from them to an AI service, a cloud-based tool or any other third party (section 6). You are not paid for taking part.

Apple runs TestFlight. Through it I also see your name and email address, which build you installed, your usage such as sessions and crashes, and any feedback you send, whether or not you donate (section 4.5). I delete feedback and crash reports once answered, and at the latest 12 months after I receive them (section 8).

## Google Drive and AI services: only with your written YES

Nothing in this section happens unless you agree in writing. The app does not ask you this (section 11).

- **How I ask.** By email (`kinetwin-participant-consent-2`). Box A asks whether I may keep your data in my personal Google Drive, in a folder only I can open, and on my own computer while analysis runs. Box B asks whether I may send it to Google Antigravity, Anthropic Claude (including Claude Code), or OpenAI ChatGPT and Codex. You answer YES or NO for each service separately. A service you do not answer YES is a no (sections 1, 6). Every box is optional, and saying no changes nothing about your place in testing (section 5). Please put your donor ID in your reply, so I know which files are yours (section 4.3).
- **If you do not reply YES,** nothing changes: your data stays as this sheet describes, and no AI service receives it (section 1).
- **What for.** To develop and test Kinetwin's analysis and models: to check and improve the analysis and write the code. The legal basis is your explicit written consent (sections 5, 6).
- **Who.** Google Drive and Google Antigravity: Google Ireland Limited. Anthropic Claude: Anthropic Ireland, Limited. OpenAI ChatGPT and Codex: OpenAI Ireland Limited. In Antigravity I use only Google's Gemini models for your data, unless you also answered YES for Anthropic (section 6). These companies are in Ireland, in the EU, and may also process data in the USA under their own safeguards. Your data is not sent to any other AI service, and in particular not to any service that stores data in China (section 7).
- **What that means.** These are consumer services on my personal accounts. Each company handles what I send under its own terms and privacy policy, as its own controller. There is no contract between the company and me about your data, and its staff may look at it, for example for safety checks. Google Drive is also on my personal account: Google stores the files under its own terms and privacy policy (section 6).
- **Training.** Before sending anything I switch off, wherever the service offers it, the setting that lets the company train its AI on my chats: "telemetry" in Antigravity, "Help improve Claude" in Claude, "Improve the model for everyone" in ChatGPT. Google still uses what I send to run the service and keep it safe. Anthropic can keep chats flagged by its safety systems for up to 2 years and use them even with training off; I cannot undo that (sections 6, 8).
- **Before anything goes.** I label your data with a participant code, not your name. Before a video goes to an AI service, I remove its sound and location data and crop or blur anyone else who can be recognised in it (sections 4.8, 6).
- **How long.** Copies in my Google Drive, on my computer and in chats with the AI services have no fixed end date. I keep them as long as I develop Kinetwin's analysis and models with them, and delete them when you ask me to or when I stop developing Kinetwin, whichever comes first. Each year I check whether I still need them, and I ask you each year to confirm. I stop sending data to these consumer AI services when Kinetwin is released to the public. Your files in the Cloudflare storage still follow the 730 days (sections 1, 8).
- **What each company keeps.** Google Antigravity keeps it until I ask Google to delete it. Anthropic: chats I delete are removed within 30 days; flagged chats, see Training. OpenAI: chats I delete are removed within 30 days, longer if OpenAI must keep them for safety or legal reasons. Google Drive: files I delete are removed by Google under its own terms and privacy policy (section 8).
- **Withdraw.** Email kinetwin@proton.me, or reply to my consent email. You can withdraw any box on its own. From then on I send nothing more to that service, and within 30 days I delete the chats that contain your data and ask the company to delete what it kept. Withdrawing does not undo what happened before (section 9).
- **Delete.** Email kinetwin@proton.me. I then delete your copies in Google Drive and on my computer and the chats that contain your data, and ask each company to delete what I sent (section 9).
- **The app does not reach these copies.** **Leave the beta** and **Delete my data** do not tell me, so they do not reach Google Drive or the AI services: email me as well (section 9).

The consent screen in the app (quoted below, and fixed) says your data is "not shared with anyone for their own use" and that "Everything is deleted automatically after about 24 months (730 days)". If you answer YES by email, the services you chose do receive your data, as their own controllers, and your copies in Google Drive and with those services follow "How long" above instead. Your files in the Cloudflare storage still follow the 730 days (sections 5, 6, 8).

## Google Cloud and model training: only with your written YES

Nothing in this section happens unless you agree in writing. The app does not ask you this (section 11).

- **How I ask.** By email (`kinetwin-beta-cloud-training-addon-2`), with two separate boxes. Box C1: may I store your donated clips and the data Kinetwin makes from them on Google Cloud servers in the EU (Netherlands) and run the analysis there? Box C2: may I use them to train and test Kinetwin's own AI models, which are built into the app on users' phones? A box you do not answer YES is a no; if you do not reply, nothing changes (sections 1, 5).
- **Who and where.** Google Cloud EMEA Limited (Ireland) works for me under a data processing agreement and may use your data only on my instructions. Your data is stored in europe-west4 (Netherlands). Before any other cloud company receives your data, I email you and use it only if you reply YES (sections 6, 7).
- **How long.** Copies on Google Cloud and training sets are deleted at the latest about 730 days after the original upload. Models already trained with your clips can stay in use after that; if you withdraw Box C2, section 8 says what happens to them (section 8).
- **Withdraw** either box on its own by email. It stops only that use; your donation stays until you delete it in the app or it expires. **Leave the beta** and **Delete my data** do not reach Google Cloud or my training sets: email me as well (section 9).

## Your choices, any time, in Beta settings

- **Stop donating**: stops uploads and removes clips still waiting on your phone. It keeps what you already uploaded and does not withdraw your consent for those clips; they stay until you delete them or they expire.
- **Delete my data**: asks the server to delete everything stored under your donor ID, removes clips still waiting on your phone and then gives you a new random ID. **It also turns donating off.** Until the server confirms the deletion, Beta settings says your earlier data is still being deleted, you cannot turn donating on, and the app retries each time you open it (or when you tap **Retry deletion**). If the server refuses, the app asks you to email me.
- **Leave the beta**: withdraws both consents at once, stops uploads, removes clips still waiting on your phone and then deletes your data. Kinetwin stays usable afterwards. If you are offline, the consent is still withdrawn and the app retries the deletion each time you open it. **Keep Kinetwin installed until Beta settings no longer says that your earlier data is still being deleted;** if you delete the app first, the retry is lost. Leaving in the app does not tell me and does not remove you from TestFlight: email me, or stop testing in the TestFlight app.
- To donate again after any of these, you tick both boxes again.
- None of these reach Google Drive or the AI services: email me for those (previous section).
- **Your donor ID** is shown in Beta settings. Keep it if you want to ask me for a copy of your data. There is no export in the app, so I prepare the copy by hand. A donor ID is not a secret, so for requests by email I also ask for two things only you would know, for example your device model and the approximate date and length of one clip (section 9).
- You can also email kinetwin@proton.me to ask for a copy, a correction or a restriction, or to object. I answer within one month, and requests are free. You can complain to the Autoriteit Persoonsgegevens (https://autoriteitpersoonsgegevens.nl) or to the authority where you live or work (section 9).

No model is trained on your clips unless you answer YES to Box C2 of my cloud and training email, and I test each recipe in writing before it is used on donated clips. Data you delete drops out of all later training; for models already trained, section 8 says what happens.

Delete before you uninstall. If you delete the app without deleting your data, your files stay until they expire after about 730 days, and I may not be able to tell which are yours. A TestFlight build also stops opening after at most 90 days; after that, email me at kinetwin@proton.me to use any of these choices (section 9).

## Please

- Film only yourself. Keep other people out of the picture. If you appear in someone else's clip, email me at kinetwin@proton.me and I will look for it and delete it (section 4.8).
- Remember a donated clip can identify you. Do not donate if that is a problem for you.
- Do not put personal details into feedback, screenshots or the velocity file that you do not want me to have.

## The consent screen

The donation screen is shown the first time you open Kinetwin, and again if you choose Turn on donating in Beta settings. It does not block the app: No thanks opens Kinetwin as normal. These are the exact texts, fixed under `kinetwin-beta-consent-3`. Any change to the wording, the files collected or the purposes means a new version and fresh consent. Google Drive and the AI services are not on this screen: I ask for them only by email (section 11).

### Donation screen

**Title:** Donate clips to improve Kinetwin (optional)

**Summary shown above the boxes**

> Kinetwin works fully without donating. Nothing is uploaded unless you turn donating on and then confirm a clip.
>
> If you donate a clip, Kinetwin uploads it to private storage in the EU. The sound and the information hidden in the video file, such as location, are removed first. With the clip go what Kinetwin makes from it (body pose, 3D twin and measurements) and technical details: your device model, iOS version, app version, region, the height you type and details about the video. If you add them, your known 1RM, set load and bar-velocity file go too.
>
> Simon Pastoor is responsible for your data. He uses it to test and improve Kinetwin's pose measurement and the app, including training its models, and for research on lifting technique. Kinetwin is planned as a commercial app, so your data helps build a product. You are not paid. The data is not sold, not used for advertising and not shared with anyone for their own use.
>
> It is stored under a random ID, not your name, but your video can show your face and body. Your internet address is kept only as a one-way scrambled code, for about a day, to stop abuse. Everything is deleted automatically after about 24 months (730 days).
>
> You can stop donating, delete your data or leave the beta at any time in Beta settings. A model already trained with your data is not retrained when you delete; deleted data drops out of later training.

("Read the full privacy notice" links to https://smasher4459.github.io/kinetwin-legal/privacy/.)

**Checkbox 1: donating** (unticked by default)

> I am 18 or older. I agree that clips I choose to donate, with their analysis files, any extras I add and my device details, are uploaded to Kinetwin's private EU storage, so that Simon Pastoor can use them to test and improve Kinetwin's pose measurement and the app, including training its models, and for research on lifting technique. Kinetwin asks me before each clip is uploaded.

**Checkbox 2: explicit consent for body and fitness data** (unticked by default)

> I give my explicit consent to Simon Pastoor processing my body and fitness data for those purposes: my video, my body pose and joint positions, my height, my lifting measurements, and my 1RM, set load and bar-velocity file if I add them. I understand this may reveal information about my body and health. I can withdraw this consent at any time in Beta settings, and that does not affect what happened before.

**Buttons**

- **Turn on donating**: enabled only when both boxes are ticked.
- **No thanks, use Kinetwin without donating**: nothing is uploaded and Kinetwin opens as normal. Shown below the button: "You can change your mind later in Beta settings."

### Confirmation shown for each clip

Shown after the analysis and before anything is uploaded.

**Title:** Donate this clip?

> If you donate, Kinetwin uploads this clip and its analysis to private storage in the EU, for the uses you agreed to. The video uploads over Wi-Fi only. If you say no, nothing from this clip is uploaded.

**Buttons:** **Donate this clip** · **Don't donate this clip**

**Stored on the phone and sent with each donation:** `consentVersion = "kinetwin-beta-consent-3"` and `consentedAt` (ISO 8601, UTC) of the moment **Turn on donating** was tapped; and, for each clip, `clipConfirmedAt` (ISO 8601, UTC), the moment **Donate this clip** was tapped for that clip.

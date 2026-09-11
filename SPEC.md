# Tinig

**Author:** Troy

Open community TTS aimed at Taglish and Filipino: English and Tagalog in one sentence, Tagalog affixes on English roots (`nag-meeting`, `i-submit`, `ina-update`), Filipino accents that are not Manila-only, and the particles people actually say (`po`, `opo`, `na`, `pa`).

Standing rule, same as the other AI work: **no claim without a run.**

---

## 1. Problem

Closed Filipino TTS already talks. SpeechGen, Fliki wrappers, ElevenLabs, and the rest will read a Tagalog paragraph or a mixed line if you pay. What they get wrong for people who actually speak Taglish is the stuff that is not a clean language switch: English roots under Tagalog morphology, particles that change the sentence, and accents that are not broadcast Manila.

Open is thinner. Meta MMS ships `facebook/mms-tts-tgl` (VITS, Tagalog). It exists. It is also **CC-BY-NC 4.0**, so it is not a community commercial base, and it is Tagalog-first, not Taglish-first.

The hole is not “no Filipino TTS exists.” The hole is open, Taglish-first, accent-honest, under a license you can actually use, scored on an eval Troy cares about.

## 2. Bar

Beat a named baseline on a tiny eval set of sentences Troy (and later the community) actually care about.

First named baseline: **Meta MMS `facebook/mms-tts-tgl`**. Say so in the run note. Do not swap the baseline after hearing the clips.

The eval is the point, not a leaderboard. Mix English, Tagalog, affixed Taglish, particles, and at least one non-Manila note. Score what a listener can check: did the affix land, did the particle land, did the line stay one voice instead of two languages glued together. No MOS theater, no “sounds natural” without the set.

No claimed win without that run. A nicer demo clip is not a win.

## 3. Smallest peek

First ship is not a foundation model.

First peek, in order:

1. A written Taglish eval set. 20–40 lines. Mix English, Tagalog, affixed Taglish (`nag-meeting`, `i-submit`, `ina-update` and kin), particles (`po` / `opo` / `na` / `pa`), and one non-Manila note. Public, versioned, frozen before anyone trains against it.
2. A listen-able clip page or a local script that reads those lines (or a subset) from an existing checkpoint. Something a person can play. Not a coming-soon page.

Fine-tune only after that eval exists. A sprint that starts with “just cook a model” is out of order.

## 4. Community

Community here means a public eval set and written rules for recordings. It does not mean a Discord vibe.

Recordings need:

- Consent that says the clip will be used to train and release speech weights.
- A license that is not NC, if the goal is usable weights. CC-BY-NC on the data makes CC-BY-NC weights. Say so, or do not call it community-usable.
- A speaker note (accent, not a biography). Manila is one accent. It is not the set.

Reject clips with no consent, no license, or a license that cannot ship with the weights you claim.

## 5. Non-goals

- Not an ElevenLabs clone. No voice marketplace, no “studio quality” product surface.
- Not a voice-clone toy. Do not ship “upload a minute, get a clone.”
- Not a multi-language world model. Filipino and Taglish. Other languages wait.
- Not training until a sprint is named. This file is not permission to start a run.

## 6. License note

`facebook/mms-tts-tgl` is **CC-BY-NC 4.0**. Fine-tuning it does not wash the NC off. If a release is built on that checkpoint, the note has to say NC. Do not call that a community-usable weight.

When a sprint starts, prefer a permissive-base path (weights and data you can actually pass on). If the only honest path at that moment is NC, say NC. Silence is a lie.

Repo license for code and docs can be permissive (MIT or Apache-2.0) without pretending the MMS weights are.

## 7. 02 portfolio

This repo is the AI-engineer work object in progress.

The desk may show Tinig only when there is something to peek: a clip, or the written eval. Never a coming-soon plaque. Spec-only is for this repo, not for a tile that pretends there is a voice.

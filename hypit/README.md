# Hypit: gayahin ang structure ng viral video gamit ang AI agent mo

Kung galing ka sa comment na **HYPIT**, nasa tamang lugar ka. 👋
Karamihan ng viral video ay hindi original: inuulit nila ang structure na gumana na. Ang **Hypit** ay open-source tool na nagpapa-aral nito kay Claude Code o Codex, tapos binubuo ulit ang structure para sa **sarili mong mensahe**.

**Link:** [github.com/hypit-ai/hypit](https://github.com/hypit-ai/hypit) · [hypit.ai](https://hypit.ai)

> **Tapat na paalala (na-check noong Nobyembre 2026):** libre ang Hypit (open source, mahigit 31K GitHub stars), pero **may sariling bayad ang coding agent mo** (hal. Claude Code) at ang anumang **paid AI model** (image/video/voice generation). Hindi mo kailangan ang paid models kung sariling boses at motion graphics ang gagamitin mo. Gayahin ang **structure**, hindi ang salita, footage o music ng iba.

---

## 1. I-install

Kailangan mo ng [Node.js](https://nodejs.org) 22.15+ at [FFmpeg](https://ffmpeg.org/download.html). Sa terminal:

```text
npx skills add hypit-ai/hypit -g
```

Ito ang nag-i-install ng Hypit Skill para sa agent mo. Sa unang gamit, ang agent mismo ang tutulong i-setup ang Hypit executable (`npm install --global @hypit/hypit`).

## 2. Ipa-aral ang reference video

Ilagay ang link o file ng video na gusto mong gayahin, at sabihin sa agent mo (Claude Code o Codex):

```text
Use the hypit skill. Study this reference video: [LINK O FILE].
Explain in simple words: how the hook lands, when the captions hit, what the visuals explain,
and why it holds attention. Show me representative frames with the words spoken at that moment.
Do not use any paid generation model without asking me first.
```

## 3. Buuin ulit para sa sarili mong mensahe

```text
Now rebuild that structure for my own message:
- Topic: [TOPIC MO]
- Opening: [SARILING HOOK]
- Voice: [boses mo / voice clone / recording]
Keep the captions, b-roll and effects linked to my words, not fixed seconds.
Write the script first and wait for my OK, then make the video and show me the editable version in Hypit Studio.
```

## 4. Ang madalas hindi napapansin

Sumusunod sa **mga salita** ang captions, b-roll at effects, hindi sa nakatakdang segundo. Kapag binago mo ang script, kusang umaangkop ang workflow, kaya hindi ka na nagsisimula sa blangkong timeline.

---

[← Bumalik sa lahat ng project](../README.md)

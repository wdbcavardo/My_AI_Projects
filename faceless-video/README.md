# Faceless Video: Gumawa ng Reels nang hindi humaharap sa camera

Avatar ng mukha mo + AI clone ng boses mo + Claude Code para sa pag-edit.
Ito ang setup na ginamit ko sa mga Reels ko. Kung galing ka sa comment na **AVATAR**, nasa tamang lugar ka. 👋

> **Tapat na paalala:** may bayad ang ElevenLabs (Starter) at ang Claude Code (paid Claude plan). I-review pa rin ang bawat video bago i-post, **sariling boses lang ang i-clone**, at lagyan ng **AI label** ang post.

---

## Hakbang 1: Gawing cartoon avatar ang mukha mo

Kailangan mo lang ng isang malinaw na litrato ng mukha mo (nakaharap, maliwanag).

1. Gumamit ng AI image tool na may image generation (hal. ChatGPT o Gemini).
2. I-upload ang litrato mo at gamitin ang prompt na ito:

```text
Turn this photo into a clean black-and-white cartoon avatar of the same person.
Head only (no neck or body), facing the camera, simple bold line art, white background,
friendly neutral expression with closed mouth, keep my hairstyle, glasses and face shape.
Square image, high resolution.
```

3. I-save bilang `avatar.png`. Ulitin hanggang kamukha mo talaga.

**Tip:** mas madaling gawan ng lip-sync ang avatar kung nakasara ang bibig at malinaw ang mata.

## Hakbang 2: I-clone ang boses mo sa ElevenLabs

1. Gumawa ng account sa [elevenlabs.io](https://elevenlabs.io) at piliin ang **Starter** plan (mga $6 kada buwan; i-check ang kasalukuyang presyo sa pricing page nila).
2. **Voices → Add a new voice → Instant Voice Clone.**
3. Mag-record o mag-upload ng **1–2 minutong malinis na boses mo**: tahimik na kwarto, walang music, relaxed na parang kausap mo ang kaibigan.
4. I-check ang consent na boses mo ito, tapos i-save. Subukan sa ilang Taglish na linya.
5. Kunin ang **Voice ID** ng clone mo.

**Ikonekta sa Claude Code** (para siya na ang gagawa ng voiceover): sa folder ng project mo, patakbuhin ito sa terminal at sundan ang lalabas. Ikaw ang mag-a-approve sa browser; hindi mo kailangang kopyahin ang API key.

```text
npx -y @elevenlabs/cli@latest onboard init
```

## Hakbang 3: Si Claude Code ang bahala sa pag-edit

Una, i-setup ang AI video editor gamit ang tatlong prompt sa [`../ai-video-editor/`](../ai-video-editor/).
Pagkatapos, ilagay ang `avatar.png` sa folder ng project at gamitin ang prompt na ito:

```text
Make a vertical animated explainer Reel (1080x1920) with no camera footage.

Topic: [TOPIC]
Audience: [WHO IT'S FOR]
CTA keyword: [KEYWORD] — the viewer gets [WHAT YOU WILL SEND]

1. Write a Taglish script (45–60 seconds) with this structure:
   hook in the first 3 seconds -> the problem -> 3 clear steps -> an honest note -> CTA.
   Show me the script and wait for my OK.
2. Voiceover: use my ElevenLabs voice clone (voice ID: [VOICE ID]), one request per line,
   and get word timings. Trim the silence at the start/end of each line and shorten long
   pauses so it sounds natural, not rushed.
3. Visuals: clean motion graphics that change every 2–3 seconds and match the words being
   said, word-by-word captions with the current word highlighted, and my avatar.png
   (small in a corner, big at emotional moments) with a mouth that moves with the voice
   and natural blinking.
4. Add light background music under the voice and soft sound effects on the animations.
5. Show me still frames of each scene before the final render. Then render to "Exports",
   plus a version without music, a 1080x1920 thumbnail and a Facebook caption.
```

## Ang resulta

- Isang Reel na boses mo at mukha mo, pero hindi ka humarap sa camera.
- Bersyong may music at wala, thumbnail, at caption na handa nang i-post.
- Mga revision sa simpleng salita: "palakihin ang hook", "bilisan ang boses nang 10%", "hinaan ang music".

---

[← Bumalik sa lahat ng project](../README.md)

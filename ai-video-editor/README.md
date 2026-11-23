# AI Video Editor gamit ang Claude Code

Gawing video editor si Claude: mula sa empty folder hanggang sa tapos na Reel, gamit ang tatlong prompt.
Ang tools ang taga-cut. Ikaw pa rin ang may taste.

> Ito ang setup na ginamit ko sa mga video ko. Kung galing ka sa comment na **EDITOR**, nasa tamang lugar ka. 👋

---

## Ano ang kailangan mo

- **Claude desktop app**, at buksan doon ang **Claude Code** (hindi sa browser). Kailangan ng paid na Claude plan para sa Claude Code.
- Computer na may sapat na espasyo (mga 2–3 GB para sa tools).
- 3–5 reference videos na gusto mo ang style.

## Setup (5 minuto)

1. Gumawa ng folder sa computer mo na **`AI Video Editor`**.
2. Sa Claude desktop app: **bagong Claude Code chat → piliin ang Local → piliin ang folder na `AI Video Editor`**.
   Ngayon, kita na ni Claude ang files mo.
3. I-paste ang tatlong prompt, isa-isa at sa pagkakasunod:

| # | Prompt | Para saan |
|---|---|---|
| 01 | [Install](prompts/01-install.md) | I-install at i-test ang limang tools. Isang beses lang. |
| 02 | [Taste mo (brand sheet)](prompts/02-taste-brand-sheet.md) | 3–5 reference videos → isang original na brand sheet. |
| 03 | [I-edit bilang Reel](prompts/03-edit-into-reel.md) | Raw footage → storyboard → tapos na Reel. |

English ang mga prompt para pinakamalinaw kay Claude. Pagkatapos, puwede mo na siyang kausapin sa Taglish.
Palitan lang ang mga nasa **[BRACKETS]**.

## Ang limang tools

| Tool | Gamit | Link |
|---|---|---|
| FFmpeg | Pag-cut, pagdugtong at pag-export | https://ffmpeg.org |
| Whisper | Offline na captions (transcription) | https://github.com/ggml-org/whisper.cpp |
| yt-dlp | Pag-download ng reference videos | https://github.com/yt-dlp/yt-dlp |
| Remotion | Video at motion graphics gamit ang React | https://www.remotion.dev |
| HyperFrames | Video at motion graphics gamit ang HTML | https://github.com/heygen-com/hyperframes |

Hindi mo kailangang i-install ang mga ito isa-isa. Si Claude na ang gagawa nito sa Prompt 01, at magtatanong muna siya bago ang anumang kailangan ng admin.

## Ang folder mo pagkatapos ng setup

```
AI Video Editor/
├── Raw Footage/     ← dito ilalagay ang mga na-film mo
├── References/      ← mga reference video (pang-aral lang)
├── Exports/         ← dito lalabas ang tapos na video
├── TOOLS.md         ← listahan ng tools at kung paano gamitin
└── BRAND-SHEET.md   ← ang style mo (galing sa Prompt 02)
```

## May mali? Sabihin mo lang.

Pagkatapos ng unang edit, kausapin mo lang si Claude sa simpleng salita:

- "Palakihin ang hook."
- "Bilisan ang unang 3 segundo."
- "Tanggalin ang part tungkol sa presyo."
- "Mas malaki ang captions."

Bawat ayos ay sine-save bilang bagong bersyon (v2, v3…), kaya hindi nawawala ang luma.

## Mahalagang paalala

- **Inspired, hindi kopya.** Ang references ay pang-aral lang ng style. Huwag gamitin ang footage, music, boses o eksaktong salita ng ibang creator.
- **Lisensya ng tools:** libre ang FFmpeg, Whisper, yt-dlp at HyperFrames. Ang Remotion ay libre para sa indibidwal at maliliit na team (hanggang 3 tao); kailangan ng company license kapag mas malaki.

---

May tanong? Mag-comment sa video o i-message ako. Susunod: ang sarili kong editing style. 🎬

📄 Mas gusto mo ng PDF? [I-download ang EDITOR-3-prompts.pdf](EDITOR-3-prompts.pdf)

[← Bumalik sa lahat ng project](../README.md)

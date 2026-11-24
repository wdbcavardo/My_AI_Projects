# OpenCode: AI video editing para sa ₱0

Kung galing ka sa comment na **OPENCODE**, nasa tamang lugar ka. 👋
Ito ang step-by-step para mag-edit ng video gamit ang AI nang walang binabayarang AI subscription.

> **Tapat na paalala (na-check noong Nobyembre 2026):** ang mga libreng model sa OpenCode ay may **"Free"** sa pangalan at libre lang **for a limited time**. Nagpapalit-palit sila, kaya piliin ang kasalukuyang may "Free". Pinakabagay ito sa short-form videos (Reels, TikTok, Shorts), at laging i-review ang output bago i-post.

---

## 1. I-install ang OpenCode

1. Pumunta sa **[opencode.ai/download](https://opencode.ai/download)**.
2. I-download at i-install ang **desktop app** para sa Windows, Mac o Linux.

## 2. I-setup ang OpenCode Console at piliin ang libreng model

1. Buksan ang OpenCode at mag-sign in sa **OpenCode Console** (Google o GitHub).
2. Sa model picker, pumili ng model na may **"Free"** sa pangalan (hal. *DeepSeek V4.1 Flash Free*). Ang buong listahan: [opencode.ai/docs/console/models](https://opencode.ai/docs/console/models/).

## 3. I-install ang FFmpeg

Libreng tool ito para sa video processing: **[ffmpeg.org/download](https://ffmpeg.org/download.html)**. O sabihin lang kay OpenCode: *"Install FFmpeg for me and add it to PATH."*

## 4. Mag-edit

Ilagay ang raw video mo sa isang folder, buksan ang folder sa OpenCode, at i-paste ito (palitan ang nasa `[ ]`):

```text
Edit [raw.mp4] in this folder into a vertical 1080x1920 Reel:
1. Remove the dead air and the unnecessary parts.
2. Add word-by-word captions (big, readable, the current word highlighted).
3. Add text overlays for the key points: [KEY POINTS].
4. Add simple transitions and light effects between sections.
5. Show me the plan first. After I approve, export final.mp4 and tell me its length and size.
Use FFmpeg for all video work. Never overwrite the original file.
```

## 5. Bonus: may Claude Code video editing setup ka na?

Puwede mong gamitin ang mga **skill** mo sa loob ng OpenCode nang walang bagong setup. Binabasa ng OpenCode ang `.claude/skills` (sa project) at `~/.claude/skills` (global). Gabay: [opencode.ai/docs/skills](https://opencode.ai/docs/skills). Ang setup ko sa Claude Code: [`../ai-video-editor/`](../ai-video-editor/).

---

[← Bumalik sa lahat ng project](../README.md)

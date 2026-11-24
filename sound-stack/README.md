# Sound Stack: 3 libreng tool para may tamang tunog ang video mo kay Claude

Kung galing ka sa comment na **SOUND**, nasa tamang lugar ka. 👋
Hindi nakakarinig si Claude, kaya nanghuhula lang siya kung saan ilalagay ang tunog. Inaayos ito ng tatlong libreng tool na ito.

| # | Tool | Ano ang ginagawa | Link |
|---|---|---|---|
| 01 · Hanap | **Openverse** | Libreng library ng milyon-milyong tunog at larawan na may open license. Walang API key. | [openverse.org](https://openverse.org) |
| 02 · Lagay | **Real SFX** | Claude Code skill na naglalagay ng totoong recording sa eksaktong frame ng video mo | [github.com/Clipwing/skills](https://github.com/Clipwing/skills) |
| 03 · Check | **Earshot** | "Tenga" ni Claude: ikinukumpara ang tunog ng edit mo sa mga pro launch film; gumagawa rin ng SFX gamit ang code | [github.com/Leonxlnx/earshot](https://github.com/Leonxlnx/earshot) |

> **Bago ka magsimula:** kailangan mo ng Claude Code na naka-setup bilang video editor ([`../ai-video-editor/`](../ai-video-editor/)). May Python at Node.js dapat sa computer mo.

---

## 01 · Openverse (Hanap)

Walang kailangang i-install. Sabihin lang kay Claude:

```text
Search Openverse (https://api.openverse.org/v1/audio/) for CC0 sound effects I can use in my video:
whooshes, pops, clicks, chimes, keyboard typing and room tone. Show me 3-5 options per type
(title, length, license), then download the ones I pick into a folder called sfx-library,
one subfolder per type, and keep a CREDITS.txt with the license and source of each file.
```

**Tip:** CC0 lang para walang kailangang credit. Iwasan ang **NC** (bawal sa negosyo) at **ND** (bawal i-cut/i-loop).

## 02 · Real SFX (Lagay)

I-install ang skill (sa terminal):

```text
git clone https://github.com/Clipwing/skills.git clipwing-skills
mkdir -p ~/.claude/skills
cp -R clipwing-skills/skills/real-sfx ~/.claude/skills/
```

Tapos sabihin kay Claude:

```text
Use the real-sfx skill. Add my sfx-library folder as the main library and index it.
Then sound-design my video: find every moment that needs a sound, put a real recording on the exact frame,
keep my voice-over and music (pass them as base_audio stems, never drop them), keep the SFX under my voice,
and run the critique loop until every axis is 8+. Save it as a NEW file.
```

**Tapat na paalala:** 78 UI sound lang ang kasama nito, kaya **Openverse muna**.

## 03 · Earshot (Check)

I-install (sa terminal):

```text
pip install "earshot[listen] @ git+https://github.com/Leonxlnx/earshot"
earshot doctor --fetch
```

Mga 3 GB ang download (kasama ang listening models). Tapos sabihin kay Claude:

```text
Run "earshot critique" on my finished video and explain the verdict and the FIX FIRST list in simple words.
Check especially that my voice and my music are present. Fix the critical and major issues, then run it again.
```

**Totoong nangyari sa akin:** nawala ang boses at music sa mix ko, at hindi ito napansin ni Claude. Nahuli ito ng Earshot (Boses 0%, Music 13%). Pagkatapos ayusin: **launch-grade**.

---

Paalala: pakinggan mo pa rin ang final video sa headphones at sa phone speaker bago i-post. Hindi pa rin nakakarinig si Claude; sukat lang ang Earshot.

[← Bumalik sa lahat ng project](../README.md)

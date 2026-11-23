# Reel Stack: 3 layer para hindi magmukhang AI slop ang Reels mo

Kung galing ka sa comment na **STACK**, nasa tamang lugar ka. 👋
Ito ang tatlong layer na ginagamit ko sa bawat animated na Reel na ginagawa ko gamit ang Claude Code.

| Layer | Ano ito | Kapag wala ito |
|---|---|---|
| **01 Brand base** | Font, kulay at mukha (avatar) na naka-lock | Iba-iba ang itsura ng bawat video, halatang AI |
| **02 Script playbook** | Structure ng script na napatunayan nang gumagana | Nanghuhula ka kung paano magsisimula |
| **03 Quality check** | Pagsilip sa bawat eksena bago mag-render | Lumalabas ang maling bigkas, sobrang habang text at maling subtitle |

> **Bago ka magsimula:** kailangan mo ng Claude Code (paid Claude plan) na naka-setup bilang video editor. Sundan muna ang [`../ai-video-editor/`](../ai-video-editor/). Kung gusto mong gamitin ang mukha at boses mo nang hindi humaharap sa camera, tingnan ang [`../faceless-video/`](../faceless-video/).

---

## Layer 1: Brand base

Isang beses mo lang ito gagawin. Sine-save ito ni Claude bilang "brand file" na susundan ng bawat susunod na video.

```text
Help me lock in my brand base for all my future Reels. Save it as brand.md in this project.

1. Fonts: one bold sans-serif for headlines and one accent font for emphasis (suggest free Google Fonts).
2. Colors: one background, one text color, and ONE accent color. Give me hex codes.
3. Face: use my avatar.png (head only) as the recurring character, small in a corner
   and big at emotional moments.
4. Layout rules: where the headline, visuals, avatar and subtitles go on a 1080x1920 frame.

Show me a sample frame first. Once I approve, every video must follow brand.md.
```

**Tip:** isang accent color lang. Kapag marami, nawawala ang "itsura mo."

## Layer 2: Script playbook

Ang structure na paulit-ulit mong gagamitin. Hindi mo na kailangang manghula kung paano magsisimula.

```text
Save this as playbook.md and use it for every Reel script I ask for:

1. HOOK (first 3 seconds): name the viewer's pain or a surprising claim. No greetings.
2. PROBLEMA: why it matters, in one or two lines.
3. 3 STEPS: give the framework a name, then explain each step as "without it -> with it".
4. CTA: one keyword to comment, and what they will get.

Rules: Taglish, conversational, 45-70 seconds, short lines, one idea per line.
Now write a script about [TOPIC] for [AUDIENCE] using this playbook. Show it to me and wait for my OK.
```

**Tip:** kapag may Reel ng ibang creator na nag-viral, ipa-breakdown kay Claude ang structure nila at idagdag sa playbook mo. Gayahin ang **structure**, hindi ang mga salita.

## Layer 3: Quality check

Bago ang mahabang render, silipin muna ang bawat eksena. Ulitin lang ang pumalya.

```text
Before rendering the final video:

1. Take a still frame of every scene and show them to me.
2. Check each frame for: text that overflows or gets cut off, overlapping elements,
   subtitles that don't match the voice, and words that are mispronounced.
3. List every problem you find, fix only those scenes, and show me the fixed frames.
4. Only render the full video after I approve.
```

**Tip:** kapag mali ang bigkas ng AI voice, ang **binibigkas** lang ang baguhin (hal. "C-T-A", "e-peyst"). Huwag galawin ang subtitle.

---

## Ang resulta

- Bawat video ay mukhang galing sa iisang channel.
- Mabilis kang makagawa ng script dahil may playbook ka na.
- Mas kaunti ang render na sayang, dahil nahuhuli agad ang mali.

Paalala: i-review pa rin ang bawat video bago i-post, at lagyan ng **AI label** kung AI ang boses o visuals.

[← Bumalik sa lahat ng project](../README.md)

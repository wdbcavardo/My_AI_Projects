# Prompt 03: I-edit bilang Reel

Mag-film gaya ng dati, ilagay ang file sa **Raw Footage**, tapos i-paste ito. Puputulin ang dead air, lalagyan ng captions at music, at ipapakita muna sa iyo ang storyboard bago mag-render.

**Paano:** palitan ang `[FILE NAME]`, tapos i-paste nang buo.

```text
Edit [FILE NAME] from "Raw Footage" into a vertical Reel (1080x1920) using
BRAND-SHEET.md.

Storyboard first, then render:
1. Transcribe it with Whisper. Find the strongest hook in what I said and suggest it as
   the opening.
2. Cut the dead air, long pauses, filler words and repeated takes. Keep the story clear.
3. Show me a storyboard before rendering: each section with timestamps, the on-screen
   text, captions, graphics/motion, and the music and sound effects. Wait for my OK.
4. After I approve: add captions in my brand style, motion graphics where they help
   explain, background music (royalty-free or mine only) and light sound effects, with
   my voice always clearly on top.
5. Render to "Exports" with a new file name. Never overwrite my raw footage or earlier
   exports.
6. Check the export (length, resolution, audio) and tell me where it is.

After that I will give you changes in plain words, for example "make the hook bigger" or
"cut the part about pricing". Apply them and save each version as a new file (v2, v3...).
```

## May mali? Sabihin mo lang.

- "Palakihin ang hook."
- "Bilisan ang unang 3 segundo."
- "Tanggalin ang part tungkol sa presyo."
- "Mas malaki ang captions."

Bumalik sa [README](../README.md)

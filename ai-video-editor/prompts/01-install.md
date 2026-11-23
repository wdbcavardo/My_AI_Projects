# Prompt 01: Install (isang beses lang)

Ini-install at tine-test ni Claude ang limang tools: **FFmpeg** (cut at export), **Whisper** (captions), **yt-dlp** (reference videos), **Remotion** at **HyperFrames** (video at motion graphics).

**Paano:** buksan ang Claude Code chat na nakakonekta sa folder na `AI Video Editor`, tapos i-paste ito nang buo.

```text
Be my video editor. This folder is our editing workspace.

1. Create these subfolders if they don't exist: "Raw Footage", "References", "Exports".
2. Check what is already installed on this computer, then install and test these tools.
   Prefer installing them inside this folder (or a local virtual environment) instead of
   system-wide, and ask me before anything that needs admin rights:
   - FFmpeg (cutting, joining, exporting)
   - Whisper (offline transcription for captions; use whisper.cpp or faster-whisper,
     whichever works here)
   - yt-dlp (downloading my reference videos)
   - Remotion and HyperFrames (building the video and motion graphics)
3. Test each tool with a tiny real job (for example: export a 3-second test clip,
   transcribe a short audio sample) and show me the result.
4. Write a short TOOLS.md in this folder: what is installed, where, the version, and the
   exact command to run each one.

Do not delete or overwrite anything in "Raw Footage". When you finish, give me a checklist
of what works and what still needs my action.
```

**Tip:** puwedeng humingi si Claude ng pahintulot bago mag-install. Basahin muna bago pumayag. Kapag may pumalya, i-paste lang ang error at sabihing "ayusin mo ito".

Susunod: [Prompt 02: Taste mo](02-taste-brand-sheet.md)

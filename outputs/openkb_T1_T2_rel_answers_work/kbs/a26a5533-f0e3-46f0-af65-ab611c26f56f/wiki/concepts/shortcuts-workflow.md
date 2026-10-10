---
type: "Concept"
sources: ["summaries/session-34_2024-12-16.md"]
description: "An iPhone Shortcut that routes podcast clips, TTS highlights, and voice notes into one Apple Notes hub."
---

# Shortcut‑Based Audio Hub Workflow

**Definition**: A minimalist, audio‑first system that uses [[entities/apple-shortcuts]] on the [[entities/iphone]] to collect podcast excerpts, text‑to‑speech excerpts, and voice‑note takeaways into a single [[entities/apple-notes]] file (often called an “Audio Inbox”).

---

## Overview
The workflow automates the capture and centralisation of auditory learning material, reducing screen interaction and supporting eye‑friendly consumption. It builds on the principles of [[concepts/active-listening]], [[concepts/selective-note-taking]], and an audio‑first review loop.

---

## Core Steps
1. **Create an Audio Inbox** – open [[entities/apple-notes]] and make a note titled *Audio Inbox*.
2. **Build the Shortcut** – using [[entities/apple-shortcuts]], create a share‑sheet shortcut (often called *Append to Audio Inbox*) that:
   - Accepts incoming files, text, or audio.
   - Prepends a timestamp.
   - Appends the content to the designated note.
3. **Capture Podcast Clips** – in apps like [[entities/overcast]] or [[entities/airr]], save a clip, then share it to the shortcut. The clip lands as an embedded audio file in the inbox.
4. **Add TTS Highlights** – from [[entities/voice-dream-reader]] (or Apple’s *Speak Screen*), highlight an excerpt, share it, and the shortcut stores the text block.
5. **Record Voice Takeaways** – use [[entities/noted]] or [[entities/audio-pen]] to record a thought, optionally let the app transcribe, then share to the shortcut. Both the raw audio and its transcript are appended.

---

## Review Process
- Open the single note.
- Activate *Speak Screen* (or ask Siri) to read any text blocks.
- Tap any embedded audio file to listen.
- No folder navigation; everything is consumed from one place, keeping visual demand low.

---

## Benefits
- **Audio‑first**: minimizes visual scrolling.
- **Consistent capture**: all learning artifacts live together.
- **Automation**: a single shortcut handles every source, reducing manual organization.
- **Scalable**: works with any app that supports iOS sharing.

---

## Related Concepts
- [[concepts/shortcuts-workflow]] – general design pattern for using Shortcuts to automate content pipelines.
- [[concepts/active-listening]] – the intentional listening practice that the workflow supports.
- [[concepts/selective-note-taking]] – brief recaps or voice notes that are captured via the shortcut.
- [[concepts/text-to-speech]] – feeding TTS excerpts into the hub.

---

## Source
This concept is derived from the recommendations in [[summaries/session-34_2024-12-16]].
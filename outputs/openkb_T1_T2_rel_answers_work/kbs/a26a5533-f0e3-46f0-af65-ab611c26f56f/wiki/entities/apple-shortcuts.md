---
sources: ["summaries/session-34_2024-12-16.md"]
type: "Product"
description: "Apple's iOS app for building custom automation shortcuts."
---

# Apple Shortcuts

Apple Shortcuts is a built‑in iOS **product** that lets users create custom automation workflows. In the context of [[summaries/session-34_2024-12-16]], it is used to build a **[[concepts/shortcuts-workflow]]** that gathers audio clips, text‑to‑speech highlights, and voice‑note recordings into a single hub.

## Key facts from session‑34
- A Shortcut named *Append to Audio Inbox* is placed in the Share Sheet, accepting audio, text, or files from other apps.
- The Shortcut timestamps each item and appends it to an [[entities/apple-notes]] file (the “Audio Inbox”).
- This workflow enables an **audio‑first** review process on an [[entities/iphone]] without heavy screen interaction.
- Apps such as [[entities/overcast]] (podcast clipping), [[entities/noted]] or [[entities/audio-pen]] (voice‑note capture), and [[entities/voice-dream-reader]] (text‑to‑speech) can all share directly to the Shortcut, centralising content.

## Related concepts and entities
- [[concepts/shortcuts-workflow]] – the overarching design pattern of using Shortcuts to streamline content aggregation.
- [[concepts/text-to-speech]] – leveraged by Voice Dream Reader and Apple’s Speak Screen, with highlights routed through the Shortcut.
- [[entities/iphone]] – the hardware platform where Apple Shortcuts runs.
- [[entities/apple-notes]] – the destination note that acts as the unified audio hub.
- [[entities/overcast]], [[entities/noted]], [[entities/audio-pen]] – source apps that feed content into the Shortcut.

## Usage overview
1. Create an Apple Notes file (e.g., *Audio Inbox*).
2. Build an **Apple Shortcuts** workflow that accepts shared items, adds a timestamp, and appends them to the note.
3. In supporting apps, use the Share → *Append to Audio Inbox* action to funnel podcast clips, TTS highlights, or voice recordings.
4. Review the consolidated note by tapping audio files or using Speak Screen to read any appended text.

This setup exemplifies how Apple Shortcuts can serve as a lightweight, audio‑centric integration layer for personal learning workflows.
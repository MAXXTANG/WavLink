# WavLink

**WavLink** is a browser-based audio concatenation tool built by [Studio HAN](https://github.com/MAXXTANG). Upload multiple WAV or MP3 files, arrange them in any order, and merge them into a single audio file — all processed locally in your browser. Your files never leave your computer.

> Brewing sounds, serving peace.

## Features

### Core
- **Drag & drop upload** — drop WAV/MP3 files or click to browse (supports 12+ files)
- **Drag-to-reorder** — rearrange tracks intuitively with SortableJS
- **Per-track playback** — preview individual tracks with animated playhead
- **Export formats** — lossless WAV or compressed MP3 (128–320 kbps)
- **Progress indicator** — real-time progress bar during merge

### Audio Processing
- **Trim** — drag handles on waveform or type exact start/end times per track
- **Crossfade** — smooth transitions between tracks (0–5s)
- **Fade In / Fade Out** — gradual start and end for the final output (0–10s)
- **Gap / Silence** — insert silent intervals between tracks (0–5s)
- **Volume normalization** — auto-normalize all tracks to consistent loudness

### Workflow
- **Canvas waveform** — real-time waveform visualization for every track
- **Custom filename** — name your export, or use Studio HAN naming templates
- **Zero server dependency** — 100% client-side with Web Audio API + lamejs

## Usage

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari)
2. Drag audio files into the upload zone
3. Reorder, trim, and adjust settings
4. Click **"Start Merge"**
5. Preview the result and download

No installation, no server, no signup required.

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Audio engine | Web Audio API (decode, trim, crossfade, normalize, resample) |
| MP3 encoding | [lamejs](https://github.com/zhuker/lamejs) via CDN |
| Drag & drop sorting | [SortableJS](https://sortablejs.github.io/Sortable/) via CDN |
| Waveform rendering | Custom Canvas 2D |
| UI | Vanilla HTML5, CSS3, JavaScript (no framework) |

## Privacy

All audio processing happens entirely in your browser. No files are uploaded to any server. No data is collected or transmitted.

## License

[MIT](./LICENSE)

---

*Built with care by Studio HAN / han.wav*

# EverCut Pro 🎬

EverCut Pro is a premium, professional-grade non-linear web video editor built entirely in a single HTML file using React, Web Audio API, Canvas 2D, and Tailwind CSS. It is designed to match the UI conventions and functionality of modern desktop NLEs (like DaVinci Resolve, Premiere Pro, and Final Cut Pro).

## 🚀 Key Features

* **Slate-Dark Glassmorphic UI**: Tailored slate dark mode colors, frosted glass effects, and Outfit/JetBrains Mono typography for a state-of-the-art NLE editor aesthetic.
* **Collapsible Left Media Library Panel**: Import local video, audio, and image assets. Rendered as cards with metadata, with drag-and-drop or single-click timeline insertion.
* **Collapsible Right Inspector Panel**: Edit properties for the selected clip:
  * *Video/Image*: Volume, speed presets (0.5x to 2x), and visual filters (Brightness, Contrast, Saturation, Hue Rotate, and Blur).
  * *Audio*: Volume, playback speed, and customizable Fade In / Fade Out transition curves.
  * *Text*: Content textarea, Font Family dropdown, color picker, size, and custom X/Y positioning coordinates.
* **Custom Stereo VU Level Meter**: Real-time dual-channel (L/R) stereo meter using a `ChannelSplitterNode` off the audio destination, complete with peak holds, decay timers, and dB tick marks (from `-40dB` to `0dB`).
* **Timeline Snap Guides**: Intelligent yellow guide lines that overlay the timeline, automatically highlighting snap points when clips, markers, or the playhead are dragged near target boundaries.
* **Diamond-Head Playhead Needle**: A custom ruby-red playhead that sweeps across all timeline tracks for frame-accurate editing.
* **Interactive Export Modal**: Renders the active timeline selection with real-time percentage indicators, active rendering frames, and remaining time (ETA) estimates.

---

## 🛠️ Technology Stack

1. **Framework**: React (v18.2.0) loaded dynamically via Babel Standalone.
2. **Styling**: Tailwind CSS (CDN) coupled with custom standard CSS scrollbars and native WebKit fallbacks.
3. **Icons**: Lucide Icons.
4. **Media Engine**: Canvas 2D Context + Web Audio API.

---

## 📥 How to Run Locally

You can launch EverCut Pro by running a simple local HTTP server:

```bash
# Using Python
python3 -m http.server 8000
```

Then open `http://localhost:8000/index.html` in your web browser.

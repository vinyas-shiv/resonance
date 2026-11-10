# 🎛️ Resonance Pro

**Slowed & Reverb. Reimagined.**

[Live Demo](https://www.google.com/search?q=https://vinyas-shiv.github.io/resonance/)

[Zero Backend](https://www.google.com/search?q=https://vinyas-shiv.github.io/resonance/)

**Resonance** is a modern, zero-latency browser audio studio built for creating **Slowed + Reverb**, **Nightcore**, **Daycore**, and **Vaporwave** remixes. Engineered entirely on the client side using the Web Audio API, Resonance processes and masters audio tracks directly on your device—with zero server uploads, zero compression artifacts, and instant lossless WAV export.

👉 **Launch the Live Studio:** [**https://vinyas-shiv.github.io/resonance/**](https://www.google.com/search?q=https://vinyas-shiv.github.io/resonance/)

## ✨ Key Features

* **Precision Tempo & Pitch Resampling** — Smooth playback speed control (`0.50x` to `1.50x`) paired with independent semitone pitch detuning (`-12 st` to `+12 st`) and quick-snap tempo pills.

* **Algorithmic Convolution Reverb** — Custom-synthesized impulse response engine featuring five distinct acoustic spaces (*Empty Cathedral*, *Concert Hall*, *Ethereal Dream*, *Cozy Bedroom*, and *Submerged Void*) with adjustable wet/dry mix and decay tails up to `9.0s`.

* **808 Sub-Bass & Tone Sculpting** — Dedicated low-shelf equalizer boost (`120 Hz`, up to `+15 dB`) for warm, punchy low-end weight alongside a high-cut damping filter (`1.5 kHz` to `20 kHz`) for vintage tape warmth.

* **Procedural Vinyl & Cassette Texture** — Built-in pink/brown noise and vinyl crackle generator with adjustable texture gain.

* **One-Click Studio Presets** — Instant sound profiles including *Slowed + Reverb*, *Nightcore*, *Daycore / Heavy*, *Vaporwave '88*, *Underwater*, *Cathedral Void*, and *Clean Studio*.

* **Real-Time Acoustic Visualizer** — 60fps HTML5 Canvas spectrum analyzer with switchable **Bars** (frequency spectrum) and **Wave** (oscilloscope) views, plus an instant **Bypass FX** toggle to A/B test against the original track.

* **Lossless 16-Bit PCM WAV Export** — High-speed `OfflineAudioContext` rendering engine that bounces your full remixed track (including the complete reverb tail) into a studio-quality stereo `.wav` file in seconds.

* **Built-In Synthwave Demo Generator** — Test every slider and reverb space immediately with a single click using the procedural in-browser *Demo Track* synthesizer.

## 🛠️ Architecture & Tech Stack

| Layer | Technology | Purpose | 
| ----- | ----- | ----- | 
| **Audio DSP** | [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) (`AudioContext`, `OfflineAudioContext`) | Real-time node graph, Biquad filters, Convolver reverb, and offline WAV rendering | 
| **Visualizer** | [HTML5 Canvas 2D API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) + `AnalyserNode` | 60fps real-time frequency bar and time-domain waveform rendering | 
| **UI & Styling** | [Tailwind CSS](https://tailwindcss.com/) + Custom Frosted Glass CSS | OLED black theme (`#000000`), translucent bento-grid cards, and tactile sliders | 
| **Hosting** | [GitHub Pages](https://pages.github.com/) | 100% static, serverless delivery with zero backend infrastructure | 

## 🚀 Running Locally

Because **Resonance** is built as a zero-dependency, single-file static application, no build tools (`npm`, `webpack`, or `vite`) are required:

1. Clone the repository:

   ```
   git clone https://github.com/vinyas-shiv/resonance.git
   
   ```

2. Open `index.html` directly in any modern web browser (Chrome, Safari, Edge, or Firefox).

## 🔒 Privacy by Design

Your audio files never leave your computer. All file decoding, DSP filtering, convolution reverb, and WAV encoding execute strictly inside your browser's local memory.
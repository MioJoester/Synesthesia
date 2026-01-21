# Synesthesia

Synesthesia is an experimental, open-source audio visualization project that transforms sound into immersive, real-time 3D particle motion. It explores the relationship between audio frequencies and visual form using modern web technologies.

The project supports both **file-based audio visualization** and **live microphone input**, each implemented as a dedicated page for stability and clarity.

---

## Modes



### File-based Visualizer
<img src="/Asset/file.png" />

- Drag and drop MP3 or audio files
- Frequency analysis using the Web Audio API
- Ideal for offline experimentation

### Mic-based Visualizer
<img src="/Asset/mic.png" />
- Uses live microphone input
- Real-time response to voice, claps, or ambient sound
- Requires HTTPS or localhost due to browser security policies

Each mode lives on its own page to avoid audio graph conflicts and ensure consistent behavior.

---

## How It Works

1. Audio is captured either from a file or microphone
2. The Web Audio API performs FFT (Fast Fourier Transform) analysis
3. Frequency data drives particle displacement and motion
4. Three.js renders a GPU-accelerated 3D particle field
5. Visual output updates every animation frame in real time

---

## Tech Stack

- JavaScript (ES6+)
- Web Audio API
- Three.js
- Tailwind CSS
- particles.js
- HTML5


---

## Project Structure

```text
/
├─ Mic.html         # Microphone-based visualizer
├─ index.html       # Home page
├─ mp3.html         # File-based visualizer
```

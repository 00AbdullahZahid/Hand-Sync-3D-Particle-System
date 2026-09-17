# Hand-Sync Particle Nexus

An interactive real-time 3D particle experience controlled by hand gestures, powered by Three.js and MediaPipe Hands.

[![Live Demo](https://img.shields.io/badge/Live-Demo-00f2ff?style=for-the-badge)](https://00AbdullahZahid.github.io/Hand-Sync-3D-Particle-System/)
![Three.js](https://img.shields.io/badge/Three.js-black?style=for-the-badge&logo=three.js)
![MediaPipe](https://img.shields.io/badge/MediaPipe-FF4D4D?style=for-the-badge)

## Features

- Up to 20,000 animated particles, with a lower count selected automatically on mobile
- Real-time hand tracking through the webcam
- Eight particle formations:
  - Sphere
  - Heart
  - Saturn with rings
  - Flower
  - Fireworks
  - Cube
  - Helix
  - Galaxy
- Formation transitions through pinch gestures or the on-screen `Next formation` button
- Particle rotation and color shifts based on hand position
- Live HUD feedback for linked, frozen, morphing, and expanded-radius states
- Responsive layout for desktop and mobile screens

## Controls

| Gesture or control | Effect |
| --- | --- |
| Move hand | Rotate the formation and shift its colors |
| Pinch | Cycle to the next formation; pinch cycling has a four-second cooldown |
| Fist | Expand the particle radius |
| One raised finger | Freeze the mesh |
| `Next formation` | Cycle immediately without the pinch cooldown |

## Getting Started

### Try the live demo

Open the [live demo](https://00AbdullahZahid.github.io/Hand-Sync-3D-Particle-System/) in a modern browser and allow camera access when prompted.

### Run locally

The project is a single static HTML file. Clone the repository and serve the folder over HTTPS or localhost so camera permissions work correctly:

```bash
git clone https://github.com/00AbdullahZahid/Hand-Sync-3D-Particle-System.git
cd Hand-Sync-3D-Particle-System
```

Then open `index.html` in a modern browser, or start any local static server. For example, with Python:

```bash
python -m http.server 8000
```

Visit `http://localhost:8000` and allow camera access.

## Technology

- [Three.js](https://threejs.org/) for WebGL rendering
- [MediaPipe Hands](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker) for hand landmark detection
- [GSAP](https://gsap.com/) loaded for animation support
- Google Fonts: Space Grotesk and DM Mono

## Requirements

- A modern browser with WebGL support
- Webcam access for gesture control
- HTTPS or localhost for the camera API

## License

Feel free to use the project for personal or commercial purposes.

Created by **Abdullah Zahid**.

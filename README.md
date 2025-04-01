# 🎧 WebXR Multichannel Audio Experience

**Immersive WebVR platform for spatial audio playback (8.1) using Three.js, GLB models, and dynamic audio streaming.**

This project creates a virtual environment in the browser where users can listen to multichannel audio sources in spatialized 3D, either through file-based playback or live audio streaming, with VR headset support via WebXR.

---

## Features

- **Immersive 3D scene** rendered in WebXR using Three.js.
- **8.1 multichannel spatial audio**:
  - 8 `SphereXXX` meshes as point sources.
  - 1 central `Socle001` mesh for low frequencies (subwoofer).
- Real-time **audio playback and analysis** using `THREE.PositionalAudio` and `AudioAnalyser`.
- Dynamic GUI (via `lil-gui`) to adjust:
  - Audio volume, cone angles, and mute settings.
  - Model and HDR environment.
  - Moebius loop visualization (reactive to sound).
-  Load multiple demos: switch between different HDRIs, GLB models, and audio sets.
- VR headset support with 6DoF movement, jumping, and flight mode.
- Audio-reactive shaders applied to an IcoSphere driven by frequency data.

---

## File Structure

webxr-audio-vr/
├── index.html
├── main.js
├── shaders/
│   ├── vertexshader.glsl
│   └── fragmentshader.glsl
├── assets/
│   ├── models/
│   │   └── arcanaTempleVR.012.glb
│   ├── hdr/
│   │   └── cloudy-sky2k.hdr
│   └── audio/
│       └── demo_001/
│           ├── Sphere001.mp3
│           ├── …
│           └── Socle001.mp3
├── README.md
└── LICENSE

---

##  Technologies Used

- [Three.js](https://threejs.org/)
- [WebXR](https://immersive-web.github.io/webxr/)
- [GLTFLoader](https://threejs.org/docs/#examples/en/loaders/GLTFLoader)
- [RGBELoader / EXRLoader](https://threejs.org/docs/#examples/en/loaders/RGBELoader)
- `lil-gui` for real-time parameter control
- Blender (for .glb environment modeling)
- Ambisonic/8.1 spatial audio techniques

---

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.

You are free to:

- **Share** — copy and redistribute the material in any medium or format.
- **Adapt** — remix, transform, and build upon the material.

Under the following terms:

- **Attribution** — You must give appropriate credit.
- **NonCommercial** — You may not use the material for commercial purposes.
- **ShareAlike** — If you remix, you must distribute your contributions under the same license.

For more details, see the [license file](LICENSE).

---

##  Author

Developed by **[Ctrl-Z & JOE]**  



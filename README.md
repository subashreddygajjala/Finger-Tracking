# Advanced AR Hand Tracking Experience

An immersive, browser-based augmented reality experience that leverages machine learning for precise, real-time hand tracking. This project combines dynamic physics, interactive audio, and modern computer vision to create a highly responsive AR environment without requiring any additional hardware beyond a standard webcam.

## Features

- **Real-Time Hand Tracking**: Utilizes Google's MediaPipe architecture to map hand skeletons and track up to 42 individual landmarks concurrently with minimal latency.
- **Gesture Recognition**: Native detection of specific gestures including precise pinches, variable hand spreading, and dynamic movement velocities.
- **Interactive Visual Physics**: Features a custom-built 2D physics engine for rendering responsive particle systems, electrical arcs, and interactive shockwaves upon gesture activation.
- **Dynamic Audio Synthesis**: Uses the native Web Audio API to modulate continuous tone pitch and volume proportionally based on the spatial distance between tracked hands.
- **Customizable Themes**: Multiple aesthetic visual pipelines (Rainbow, Cyberpunk, Lava, Ocean, Galaxy) powered by algorithmic color blending and HSL shifts.

## Technology Stack

- **Frontend**: HTML5, Vanilla JavaScript, CSS3
- **Computer Vision**: [Google MediaPipe](https://google.github.io/mediapipe/) API
- **Rendering & Audio**: HTML Canvas API, Web Audio API

## Installation & Local Development

Due to strict browser security policies enforcing HTTPS/localhost constraints for webcam hardware access, the application should be served over a local HTTP server.

1. Clone the repository:
   ```bash
   git clone <your-remote-repo-url>
   cd ar-hand-tracking
   ```

2. Start a local HTTP server:
   ```bash
   # If using Python 3
   python3 -m http.server 8000
   ```
   *(Alternatively, you can use Node's `http-server`, or the VS Code "Live Server" extension).*

3. Open your browser and navigate to `http://localhost:8000`. 
4. Grant the requested camera access permissions when prompted, and click "Enter Experience".


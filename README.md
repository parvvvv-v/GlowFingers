GlowFingers: Real-Time Gesture Visual Engine

GlowFingers is a high-performance, web-based Augmented Reality (AR) experience that transforms human hand gestures into dynamic, neon-infused digital art. Built using MediaPipe and HTML5 Canvas, it creates a seamless bridge between physical movement and visual feedback, offering a "touchless" interactive environment.

### Core Features
1. Real-Time Hand Tracking: Leverages MediaPipe’s machine learning models to track 21 hand landmarks with sub-millisecond precision.
   
2. Dynamic Visual Themes: Switch instantly between five custom-engineered visual engines:
   Rainbow: Spectral HSL cycling.
   Cyberpunk: High-contrast neon red and cyan.
   Lava: Molten, pulsating heat maps.
   Ocean: Deep-sea bioluminescence.
   Galaxy: Deep space purple and starlight effects.
   
3. Gestural Interaction: Features active "Pinch" detection that triggers shockwaves and haptic-style audio zaps.

4. Multi-Hand Synthesis: Connects two-hand interactions with interactive "energy bridges" and geometry-based rotation logic.

5. Atmospheric Audio: A built-in synthesizer generates a real-time "frequency hum" that shifts pitch and volume based on the distance between your hands.

### Technical Architecture
Frontend: HTML5, CSS3 (Custom Glassmorphism & UI animations).
Logic: Pure JavaScript (ES6+).
Computer Vision: @mediapipe/hands for skeletal hand tracking.
Graphics: Dual-canvas system (Background Matrix rain + Foreground Particle engine).
Audio: Web Audio API for real-time oscillator manipulation.

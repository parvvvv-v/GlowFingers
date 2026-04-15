## GlowFingers: Real-time Gesture Visual Engine ✨

GlowFingers is a high-performance, browser-based Augmented Reality (AR) experience that transforms your hands into a dynamic controller for light and sound. By combining advanced computer vision with interactive web technologies, it creates a "visual engine" where every movement of your fingers generates vibrant, generative art and reactive audio. 🚀

## Project Overview 🎨 

GlowFingers uses your webcam to track 21 individual hand landmarks in real-time. Instead of just "drawing," it treats your hands as emitters in a digital physics simulation. Whether you are generating "shockwaves" through pinch gestures or connecting multiple hands with high-voltage "lightning" arcs, the experience is designed to feel fluid and futuristic. ⚡

## Core Features 🌟 

1. Dual-Hand Interaction: Seamlessly tracks and visualizes two hands simultaneously with unique effects for hand-to-hand proximity.

2. Reactive Audio (Hum & Zap): Features a dynamic synthesizer that changes pitch and volume based on hand distance, plus "zap" sound effects triggered by gestures.

3. Multiple Visual Themes: Switch instantly between high-fidelity presets:
   Rainbow 🌈: Shifting spectrum colors.
   Cyberpunk 🤖: Neon reds and cyans.
   Lava 🌋: Pulsating heat signatures.
   Ocean 🌊: Deep blues and teals.
   Galaxy 🌌: Ethereal purples and cosmic glows.

4. Gesture Recognition Engine: * Pinch: Triggers shockwaves and audio zaps.

5. Spread Tracking: Monitors hand expansion (0-100%) to switch between "Fist" and "Open Hand" states.

6. Performance HUD: Real-time monitoring of FPS, hand count, and current gestures.

## Technical Concepts 🛠️ 

1. Computer Vision & Skeleton Tracking 🦴
The project utilizes MediaPipe Hands to perform sub-millisecond tracking of hand joints. By identifying specific landmarks—such as the thumb (4) and index (8) tips—the application calculates spatial data to trigger interactive events.

2. Generative Physics & Particles 🌪️
Particle Systems: Every finger tip acts as a particle emitter, leaving "glow trails" based on hand velocity.
Matrix Background: A custom "digital rain" background reacts to your hand speed; faster movements cause the matrix code to fall more rapidly.
Lightning Arcs: When two hands approach each other, the engine calculates the distance between matching fingertips and renders stochastic "electric" lines between them.

3. Web Audio API Synthesis 🎹
Unlike static sound effects, GlowFingers features a real-time Oscillator.
Frequency Modulation: The pitch is mapped to the distance between your hands.
Gain Control: The "hum" volume increases as your hands get closer, creating a physical sense of "energy".

4. Layered Canvas Architecture 🖼️
The engine uses three distinct rendering layers:
Background Canvas: Handles the Matrix code and "motion blur" trails.
Main Canvas: Renders the hand skeletons, lightning, and particle physics using screen and destination-out composite operations for a glowing effect.
Splash/UI: A separate animation loop for the futuristic "HUD" and intro screens.

## Tech Stack 💻 
Core: Vanilla JavaScript (ES6+), HTML5 Canvas
ML Framework: MediaPipe Hands
Audio: Web Audio API (Oscillators/Gain Nodes)
Styling: CSS3 Glassmorphism & Animations
Fonts: Orbitron & Rajdhani

# Scrolling Neural Network Animation Generator — Advanced

A single-file HTML5 animation generator that creates scrolling neural-network-inspired visuals using procedural shape generation, recurrent model logic, seeded randomness, canvas rendering, presets, and recording tools.

This project is designed as an experimental creative-coding playground for generative animation, neural-network-style pattern generation, abstract visual systems, and WebM recording.

---

## Features

### Core Animation System

- Fullscreen scrolling animation canvas
- Procedural shape spawning
- Neural-network-driven shape parameters
- Smooth canvas renderer for high performance
- Legacy DOM rendering mode for original-style behaviour
- Adjustable spawn rate
- Adjustable scroll speed
- Opacity decay control
- Maximum shape limit and shape cap protection
- Seeded generation for repeatable animations
- Temperature control for more or less chaotic output

---

## Neural Network Engines

The generator includes multiple network modes for producing animation parameters:

### Classic RNN

A lightweight recurrent neural network that maps random inputs and hidden state into visual properties such as:

- Shape position
- Shape size
- Shape type
- Rotation
- Scale
- Opacity
- Colour choice
- Animation style

### GRU-Attention Mode

An upgraded recurrent system using a GRU-style memory cell with lightweight attention behaviour. This creates smoother evolving patterns and more coherent sequences.

### Hybrid Memory Mode

An experimental mode designed for richer visual variation and longer-term pattern consistency.

---

## Visual Features

The animation can generate:

- Circles
- Rounded rectangles
- Triangles
- Pulsing shapes
- Rotating shapes
- Skewed shapes
- Glowing neon shapes
- Abstract node-network patterns
- Flow-field-influenced motion
- Symmetry-based compositions
- Mouse-reactive behaviour

---

## Controls

The control panel includes:

| Control | Description |
|---|---|
| Mode | Switch between Canvas and DOM rendering |
| Spawn Rate | Controls how many shapes spawn per second |
| Scroll Speed | Controls horizontal movement speed |
| Max Shapes | Limits active shapes for performance |
| Opacity Decay | Controls how quickly shapes fade |
| Palette | Chooses the colour theme |
| Seed | Makes generations repeatable |
| Temperature | Controls randomness/intensity |
| Hidden Size | Changes the neural-network hidden layer size |
| Shape Cap | Extra safety cap for shape generation |
| Start / Stop | Starts or pauses the animation |
| Reset NN | Reinitialises the network |
| Clear | Clears all active shapes |
| Record | Captures a `.webm` video |
| Download | Downloads the last recording |
| Save Preset | Saves current settings to localStorage |

---

## Presets

Presets are saved in the browser using `localStorage`.

You can save combinations of:

- Spawn rate
- Scroll speed
- Palette
- Seed
- Temperature
- Hidden size
- Shape limits
- Decay settings

Click a preset chip to load it.

Right-click a preset chip to delete it.

---

## Recording

The app can record the canvas using the browser’s `MediaRecorder` API.

### To record:

1. Click **Start**
2. Click **Record**
3. Let the animation run
4. Click **Stop**
5. Click **Download**

The output file is saved as:

```text
animation_capture.webm

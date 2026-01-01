# ⚡ 3D Reaction Timer

A visually stunning reaction time measurement game built with vanilla JavaScript and Three.js. Test your reflexes while enjoying smooth 3D animations and an immersive interactive experience.

[Live Demo](https://ivynsanpedro.github.io/reaction-game/) | [View Code](index.html)

## 📋 Overview

This portfolio project demonstrates clean code architecture, creative use of 3D graphics, and thoughtful user experience design. The game measures how quickly users can react to a visual signal, providing real-time feedback and tracking performance statistics.

## ✨ Features

### Core Gameplay
- **Precise Timing**: Measures reaction time in milliseconds using high-resolution performance API
- **Visual Signal System**: Clear 3D shape transformations indicate game states
- **Early Click Detection**: Prevents cheating by penalizing clicks before the signal appears
- **Performance Tracking**: Displays best time, average time, success rate, and total attempts

### Visual Experience
- **Dynamic 3D Scenes**: Different Three.js geometric compositions for each game state
- **Smooth Animations**: Fluid transitions, rotations, and particle effects
- **Responsive Lighting**: Color-coded lighting system that adapts to game state
- **Atmospheric Effects**: Fog, glow effects, and particle systems create depth

### User Interface
- **Modern Design System**: Clean, contemporary interface with glassmorphic panels
- **Real-time Feedback**: Instant visual and textual responses to user actions
- **Responsive Layout**: Adapts seamlessly to desktop and mobile devices
- **Accessibility Considerations**: High contrast ratios and clear visual hierarchies

## 🛠️ Technologies Used

- **HTML5** - Semantic markup structure
- **CSS3** - Modern styling with gradients, backdrop-filter, and animations
- **Vanilla JavaScript** - ES6+ features, modular architecture
- **Three.js (r128)** - 3D graphics rendering and animation
- **Google Fonts** - Inter & Space Grotesk typography

## 🚀 Getting Started

### Installation

1. Clone or download this repository
2. Open `index.html` in a modern web browser
3. No build process or dependencies required!

### Usage

1. **Start**: Click anywhere on the screen to begin
2. **Wait**: Don't click while the yellow "Wait..." message is displayed
3. **React**: Click immediately when you see the green "GO!" signal
4. **Review**: Check your reaction time and statistics
5. **Repeat**: Click "Play Again" to test yourself again

## 🎯 Project Goals

This project was designed with three strategic objectives:

### 1. Clean Code Architecture
- **Separation of Concerns**: Game logic, 3D rendering, and UI management are isolated into distinct modules
- **State Management**: Centralized `GameState` object handles all game data and transitions
- **Maintainability**: Clear naming conventions, inline comments, and logical code organization

### 2. Polished User Experience
- **Smooth Interactions**: 60fps animations with optimized Three.js rendering
- **Visual Feedback**: Every action provides immediate, clear responses
- **Intuitive Flow**: Users understand the game mechanics without instruction

### 3. Problem-Solving Demonstration
- **Edge Case Handling**: Prevents exploitation through early clicks and timeout management
- **Performance Optimization**: Efficient render loop and geometry management
- **Cross-device Compatibility**: Responsive design and touch-friendly interactions

## 🏗️ Code Architecture

### Module Structure

```
GameState
├── State management and data persistence
├── Reaction time calculations
└── Statistics tracking

SceneManager
├── Three.js scene initialization
├── 3D shape creation and animation
├── Lighting and camera management
└── State-driven visual updates

UIManager
├── DOM element references
├── State-based UI rendering
└── Statistics display updates

GameController
├── Event handling
├── Game flow orchestration
└── State transitions
```

### Key Technical Decisions

**Why Three.js r128?**
This version provides stability and broad CDN support while including all necessary features for the project's geometric animations.

**Why Vanilla JavaScript?**
Demonstrates fundamental programming skills without framework abstractions, showcasing understanding of core web APIs and DOM manipulation.

**In-Memory State Management**
All data stored in JavaScript objects rather than localStorage, ensuring consistent behavior across environments and simplifying the codebase.

**Performance API for Timing**
Using `performance.now()` provides microsecond precision for accurate reaction time measurements, superior to `Date.now()`.

**Modular Architecture**
Separating concerns into distinct managers makes the code easier to test, debug, and extend while demonstrating enterprise-level organization.

## 🎨 Design System

### Color Palette
- Background: `#0F172A` - Deep slate blue
- Surface: `#1E293B` - Lighter slate
- Accent: `#06B6D4` - Cyan
- Success: `#10B981` - Emerald
- Warning: `#FBB936` - Amber
- Error: `#EF4444` - Red
- Text: `#F8FAFC` - Off-white

### Typography
- **Primary**: Inter - Clean, modern sans-serif for UI elements
- **Display**: Space Grotesk - Geometric font for headings and emphasis

## 🔮 Future Enhancements

Potential features to demonstrate additional capabilities:

- **Difficulty Modes**: Varying delays and visual complexity
- **Sound Effects**: Audio feedback using Web Audio API
- **Leaderboard**: Persistent storage with ranking system
- **Multiplayer**: Real-time competition using WebSockets
- **Advanced Statistics**: Graphs and trend analysis using Chart.js
- **VR Support**: WebXR implementation for immersive experience
- **Custom Themes**: User-selectable color schemes and 3D models

## 📊 Performance Considerations

- **Optimized Rendering**: Minimal geometry updates per frame
- **Efficient Particle Systems**: Buffer geometry for particle effects
- **Responsive Animation Loop**: Uses `requestAnimationFrame` for smooth 60fps
- **Lazy Loading**: Three.js loaded from CDN only when needed
- **Mobile Optimization**: Reduced particle counts and simplified geometries on smaller devices

## 🐛 Edge Cases Handled

- **Early Clicks**: Detected and penalized with clear feedback
- **Rapid Clicking**: State transitions prevent exploitation
- **Timeout Cleanup**: Ensures no memory leaks from pending timers
- **Window Resize**: Scene automatically adapts to viewport changes
- **Browser Compatibility**: Tested across modern browsers

## 👤 Author

**Ivyn San Pedro**
- GitHub: [@ivynsanpedro](https://github.com/ivynsanpedro)
- LinkedIn: [Ivyn San Pedro](https://www.linkedin.com/in/ivynsanpedro/)

---

*Built with ❤️ to showcase web development skills and creative problem-solving*
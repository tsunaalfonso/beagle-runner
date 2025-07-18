# Beagle Runner - Mobile Mario-Style Game

A fun, mobile-friendly platformer game featuring a brave beagle dog as the main character. Navigate through 100 exciting levels in this Mario-style adventure!

## 🎮 Game Features

- **100 Unique Levels**: Each level has procedurally generated platforms with increasing difficulty
- **Mobile-Optimized**: Touch-friendly controls designed for mobile devices
- **Beagle Dog Character**: Cute pixelated beagle with facial features (eyes, nose, ears)
- **Mario-Style Gameplay**: Side-scrolling platformer with jumping and collision detection
- **Responsive Design**: Works on both mobile and desktop devices
- **Modern UI**: Clean, minimalist interface using Tailwind CSS

## 🕹️ How to Play

### Game Objective
Help the beagle dog navigate through platforms, avoid falling off the world, and explore all 100 levels!

### Controls

#### Mobile Controls
- **LEFT Button**: Move the beagle left
- **RIGHT Button**: Move the beagle right  
- **JUMP Button**: Make the beagle jump
- **PAUSE Button**: Pause/resume the game

#### Desktop Controls (for testing)
- **Arrow Keys** or **WASD**: Move left/right and jump
- **Spacebar**: Jump
- **P** or **Escape**: Pause/resume

### Game Mechanics
- **Physics**: Realistic gravity and collision detection
- **Lives System**: Start with 3 lives
- **Camera**: Follows the player character
- **Platform Collision**: Land on platforms to avoid falling
- **Level Progression**: Choose any level from 1-100

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation & Running

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Start the development server**:
   ```bash
   npm run dev
   ```

3. **Open your browser** and navigate to:
   ```
   http://localhost:8000
   ```

4. **Start playing**:
   - Click "Start Game" on the home page
   - Select any level (1-100) from the level selection screen
   - Use the on-screen controls to play!

## 🏗️ Technical Architecture

### Built With
- **Next.js 15** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **HTML5 Canvas** - Game rendering
- **Custom Game Engine** - Built from scratch in TypeScript

### Project Structure
```
src/
├── app/
│   ├── page.tsx              # Home page
│   ├── layout.tsx            # Root layout
│   └── game/
│       ├── page.tsx          # Game route handler
│       ├── LevelSelect.tsx   # Level selection screen
│       └── GameCanvas.tsx    # Game canvas and controls
├── lib/
│   └── gameEngine.ts         # Core game engine
└── components/ui/            # Reusable UI components
```

### Game Engine Features
- **Player Class**: Handles beagle character movement, jumping, and collision
- **Platform Class**: Manages platform rendering and collision detection
- **GameEngine Class**: Core game loop, physics, and state management
- **Level Generation**: Procedural platform generation based on level number
- **Camera System**: Smooth camera following the player
- **Error Handling**: Robust error handling and cleanup

## 🎨 Game Design

### Visual Style
- **Sky Blue Background**: Cheerful, Mario-inspired atmosphere
- **Green Ground Platforms**: Classic platformer aesthetic
- **Brown Beagle Character**: Pixelated dog with distinctive features
- **Clean UI**: Modern, mobile-first interface design

### Level Design
- **Level 1-10**: Basic platform layouts for learning
- **Level 11-50**: Increased platform complexity
- **Level 51-100**: Advanced layouts with more challenging jumps
- **Procedural Generation**: Each level has unique platform arrangements

## 📱 Mobile Optimization

### Touch Controls
- Large, easily tappable buttons
- Optimized button placement for thumbs
- Touch event handling with proper preventDefault
- No accidental scrolling during gameplay

### Responsive Design
- Full viewport canvas utilization
- Adaptive UI elements
- Safe area considerations for mobile devices
- Portrait and landscape orientation support

## 🔧 Development

### Key Components

#### GameEngine (`src/lib/gameEngine.ts`)
- Handles game loop with `requestAnimationFrame`
- Physics simulation (gravity, velocity, collision)
- Level generation and management
- Input handling and game state

#### GameCanvas (`src/app/game/GameCanvas.tsx`)
- React component wrapping the HTML5 canvas
- Mobile control overlay
- Keyboard input for desktop testing
- Error handling and cleanup

#### LevelSelect (`src/app/game/LevelSelect.tsx`)
- Grid layout of all 100 levels
- Responsive design for different screen sizes
- Navigation between home and game screens

### Performance Considerations
- Efficient canvas rendering
- Proper cleanup of animation frames
- Optimized collision detection
- Memory management for game objects

## 🐛 Troubleshooting

### Common Issues

**Game not loading?**
- Ensure you're using a modern browser with Canvas support
- Check browser console for JavaScript errors
- Verify the development server is running on port 8000

**Controls not responding?**
- On mobile, ensure you're tapping the control buttons directly
- For desktop, click on the game canvas first to focus it
- Check that JavaScript is enabled in your browser

**Performance issues?**
- Close other browser tabs to free up memory
- Try refreshing the page to reset the game state
- Ensure your device meets the minimum requirements

## 🎯 Future Enhancements

Potential features for future versions:
- **Enemies and Obstacles**: Add moving enemies and hazards
- **Power-ups**: Collectible items for special abilities
- **Sound Effects**: Audio feedback for jumps, collisions, and music
- **Animations**: Smooth character animations and particle effects
- **Multiplayer**: Local or online multiplayer support
- **Level Editor**: Allow players to create custom levels
- **Achievements**: Unlock system and progress tracking
- **Better Graphics**: Sprite-based graphics instead of simple shapes

## 📄 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features  
- Submit pull requests
- Improve documentation

## 🎉 Acknowledgments

- Inspired by the classic Super Mario Bros. platformer series
- Built with modern web technologies for optimal performance
- Designed with mobile-first principles for the best user experience

---

**Have fun playing Beagle Runner! 🐕🎮**

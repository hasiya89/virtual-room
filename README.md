# Virtual Room Designer

A modern, interactive 3D room design application built with Three.js that allows users to create and customize virtual room layouts with realistic furniture and materials.

![Virtual Room Designer](screenshots/app-overview.png)

## Features

### 🏠 Room Customization
- **Dynamic Wall Colors**: Choose custom colors for your walls
- **Multiple Wall Materials**: Brick, Wood, Modern textures, or solid colors
- **Floor Options**: Wood, Carpet, or Concrete flooring with realistic textures
- **Lighting Control**: Bright, Warm, Cool, or Dim lighting presets

### 🪑 Furniture System
- **Drag & Drop**: Intuitive furniture placement with mouse controls
- **Multiple Furniture Types**: 
  - Chairs
  - Tables  
  - Sofas
  - Beds
  - Bookshelves
  - Plants (with subtle floating animation)
- **Object Customization**: Change colors and scale of individual furniture pieces
- **Smart Positioning**: Grid-based snapping and room boundary constraints

### 🎮 Interactive Controls
- **Mouse Controls**: 
  - Left-click and drag to move furniture
  - Right-click and drag for camera orbit
  - Mouse wheel for zoom
- **Keyboard Shortcuts**:
  - `Q/E`: Rotate selected object
  - `+/-`: Scale selected object
  - `Delete/Backspace`: Remove selected object

### 🎨 Advanced Rendering
- **Realistic Lighting**: Directional and ambient lighting with shadow mapping
- **Material System**: PBR materials with texture support
- **Shadow Casting**: Dynamic shadows for enhanced realism
- **Responsive Design**: Mobile-friendly interface

## Setup Instructions

### Prerequisites
- Modern web browser with WebGL support
- Local web server (for loading 3D models and textures)

### Assets Required

The application expects the following asset structure:

```
assets/
├── models/
│   ├── bed.glb
│   ├── chair.glb
│   ├── table.glb
│   ├── sofa.glb
│   ├── bookshelf.glb
│   └── plant.glb
└── textures/
    ├── wood_floor.jpg
    ├── carpet_floor.jpg
    ├── concrete_floor.jpg
    ├── brick_wall.jpg
    ├── wood_wall.jpg
    └── modern_wall.jpg
```

### Asset Sources
- **3D Models (.glb)**: Download furniture models from [Sketchfab](https://sketchfab.com)
- **Textures (.jpg)**: Download high-quality textures from [Poly Haven](https://polyhaven.com)

### Recommended Assets

#### 3D Models (Sketchfab)
Search for and download these types of models:
- Modern chairs (office, dining, lounge)
- Tables (coffee, dining, side tables)
- Sofas and couches
- Beds (single, double, king)
- Bookshelves and storage units
- Indoor plants and planters

**Note**: Ensure models are in GLB format and appropriately sized. The application will auto-scale models, but starting with reasonable proportions helps.

#### Textures (Poly Haven)
Download these texture types:
- **Wood floors**: Oak, pine, or hardwood textures
- **Carpet**: Loop pile, cut pile, or berber textures
- **Concrete**: Smooth or textured concrete surfaces
- **Brick walls**: Red brick, painted brick, or stone textures
- **Wood walls**: Paneling, planks, or wainscoting
- **Modern walls**: Clean plaster, painted surfaces, or minimalist textures

### Installation

1. **Clone or Download** the project files
2. **Start Local Server**:
3. **Open Browser** and navigate

## Documentation Assets

### Screenshots Needed
Create these screenshots for documentation:

1. **app-overview.png** - Main interface showing the 3D room with furniture
2. **controls-panel.png** - Close-up of the control panel interface  
3. **furniture-placement.png** - Demonstrating furniture being placed/moved
4. **lighting-options.png** - Different lighting presets comparison
5. **materials-showcase.png** - Different wall and floor materials
6. **mobile-interface.png** - Mobile/responsive view

### Video Demonstrations
Consider creating these videos:

1. **quick-demo.mp4** (30-60 seconds) - Fast overview of main features
2. **furniture-placement.mp4** - Detailed furniture interaction demo
3. **customization-options.mp4** - Showing material and lighting changes
4. **full-workflow.mp4** - Complete room design from start to finish

## Browser Compatibility

- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13.1+
- ✅ Edge 80+
- ⚠️ Internet Explorer: Not supported

## Technical Architecture

### Core Technologies
- **Three.js r128**: 3D rendering engine
- **WebGL**: Hardware-accelerated 3D graphics
- **GLTF/GLB**: 3D model format
- **Web APIs**: File loading, mouse/keyboard events

### Key Components
- **Scene Management**: Room creation and lighting setup
- **Asset Loading**: Texture and model loading with fallbacks  
- **Interaction System**: Mouse picking and object manipulation
- **Material System**: Dynamic material switching and customization
- **Camera Controls**: Orbit controls and viewport management

## Performance Considerations

- Models are automatically scaled and optimized
- Textures are compressed and properly mapped
- Shadow mapping is optimized for performance
- Fallback geometry is provided when models fail to load
- Asset loading includes progress indicators

## Troubleshooting

### Common Issues

**Models not loading:**
- Ensure you're running a local server (not file:// protocol)
- Check that .glb files are in the correct assets/models/ directory
- Verify file names match exactly (case-sensitive)

**Textures not displaying:**
- Confirm texture files are in assets/textures/
- Check file formats are .jpg (not .png or other formats)
- Ensure proper server MIME type configuration

**Performance issues:**
- Use smaller texture sizes (1024x1024 or 2048x2048)
- Optimize 3D models (reduce polygon count)
- Test on different devices and browsers

## Future Enhancements

- [ ] Room size customization
- [ ] Save/load room layouts
- [ ] Additional furniture categories
- [ ] Texture customization for furniture
- [ ] Export functionality (screenshots, 3D models)
- [ ] Multiplayer collaboration
- [ ] VR/AR support

## Contributing

Feel free to contribute by:
- Adding new furniture models
- Improving the UI/UX
- Optimizing performance
- Adding new features
- Reporting bugs

## License

This project is open source. Please respect the licenses of any downloaded assets from Sketchfab and Poly Haven.

---

**Tip**: Start with free assets from both platforms to test the application, then consider purchasing premium models for production use.

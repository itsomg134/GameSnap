# GameSnap - Gaming Level Capture Extension

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

A sleek, browser-based gaming level capture tool that lets you screenshot animated game levels, manage your captures, and export them in multiple formats. Built with pure HTML5 Canvas, CSS3, and vanilla JavaScript.

![Screenshot_20-3-2026_235210_127 0 0 1](https://github.com/user-attachments/assets/7aff8ceb-9725-4de4-871e-aa2e658c8de8)

## Features

- **Real-time Level Preview** - Three beautifully animated game environments:
  -  Forest Ruins - Mystical woodland with fireflies
  -  Magma Core - Volcanic landscape with flowing lava
  -  Frost Temple - Icy shrine with falling snow

- ** Instant Screenshot Capture** - Capture any level with one click
- ** Multiple Format Support**:
  - PNG (lossless quality)
  - JPEG (compact file size)
  - WebP (modern compression)

- ** Built-in Gallery** - All captures stored locally in your browser
- ** Batch Export** - Download all captures as a ZIP file
- ** Gallery Management** - Delete individual captures or clear entire gallery
- ** Local Storage** - Captures persist between sessions
- ** Interactive Level Switching** - Seamless transition between game environments


##  Technologies Used

- **HTML5 Canvas** - Dynamic game level rendering
- **CSS3** - Glassmorphism UI design, animations, responsive layout
- **Vanilla JavaScript** - Capture logic, gallery management, ZIP export
- **JSZip** - Client-side ZIP file generation
- **LocalStorage API** - Persistent capture storage

##  Installation

### Quick Start

1. Clone the repository:
```bash
git clone https://github.com/yourusername/gamesnap-level-capture.git
```

2. Navigate to the project directory:
```bash
cd gamesnap-level-capture
```

3. Open `index.html` in your browser:
```bash
# Using Python (any version)
python -m http.server 8000

# Or simply open the file directly
open index.html
```

### No Build Required!
This is a pure frontend application with no dependencies (except optional JSZip for ZIP exports). Just open the HTML file and start capturing!

## How to Use

### Capturing Levels
1. **Select a Level** - Click on any level button:
   -  Forest Ruins
   -  Magma Core  
   -  Frost Temple

2. **Choose Format** - Select your preferred image format:
   - PNG (Best quality)
   - JPEG (Smaller size)
   - WebP (Modern compression)

3. **Capture** - Click "CAPTURE THIS LEVEL" to save the current view

### Managing Captures
- **View Gallery** - All captures appear in the right panel
- **Download Individual** - Click any gallery image to download it
- **Delete Single** - Click the trash icon on any capture
- **Export All** - Use "Download All Captures (.zip)" to get everything at once
- **Clear Gallery** - Remove all captures with one click

##  Customization

### Adding New Levels

You can easily extend the application with new game levels. Edit the JavaScript in `index.html`:

```javascript
// Add a new level drawing function
function drawSpaceLevel(now) {
  // Your custom drawing code here
  ctx.fillStyle = '#0a0a2a';
  ctx.fillRect(0, 0, canvas.width, canvas.height);
  // Add stars, planets, etc.
}

// Add to the level selection logic
else if (currentLevel === 3) drawSpaceLevel(now);
```

Then add a new button in the HTML:
```html
<button data-level="3" class="level-btn">SPACE STATION</button>
```

### Modifying Visual Styles

The UI uses CSS variables that can be easily customized:
```css
:root {
  --primary-glow: #3bc9ff;
  --dark-bg: #0a0f1e;
  --card-bg: rgba(12, 20, 30, 0.65);
}
```

##  Responsive Design

GameSnap is fully responsive and works on:
-  Desktop browsers
-  Tablets
-  Mobile devices (with touch support)

## Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 60+ |  Full Support |
| Firefox | 55+ |  Full Support |
| Safari | 12+ |  Full Support |
| Edge | 79+ |  Full Support |
| Opera | 47+ |  Full Support |

##  Project Structure

```
gamesnap-level-capture/
├── index.html          # Main application file
├── README.md           # Documentation
├── LICENSE             # MIT License
└── assets/             # (Optional) Images, icons
```

##  Privacy & Storage

- All captures are stored locally in your browser's LocalStorage
- No data is sent to any server
- Captures persist until manually deleted
- Maximum of 40 captures stored (configurable)

##  Future Enhancements

- [ ] Video recording support
- [ ] Animated GIF export
- [ ] Cloud backup integration
- [ ] Custom level editor
- [ ] Keyboard shortcuts
- [ ] Drag-and-drop reordering
- [ ] Filters and effects
- [ ] Social media sharing

##  Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Commit** your changes: `git commit -m 'Add amazing feature'`
4. **Push** to the branch: `git push origin feature/amazing-feature`
5. **Open** a Pull Request

### Development Guidelines
- Keep code vanilla JavaScript (no frameworks required)
- Maintain cross-browser compatibility
- Follow existing code style
- Test on multiple devices

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

##  Acknowledgments

- Inspired by game capture tools and screenshot utilities
- Icons and emojis for visual enhancement
- JSZip library for ZIP file generation
- Modern CSS glassmorphism trends
  
## Contact

Om Gedam

GitHub: [https://github.com/itsomg134](https://github.com/itsomg134)

Email: [omgedam123098@gmail.com](mailto:omgedam123098@gmail.com)

Twitter (X): [https://twitter.com/omgedam](https://twitter.com/omgedam)

LinkedIn: [https://linkedin.com/in/omgedam](https://linkedin.com/in/omgedam)

Portfolio: [https://ogworks.lovable.app](https://ogworks.lovable.app)

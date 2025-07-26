# Zenith Workspace

> Premium productivity desktop companion with stunning glassmorphism UI

<div align="center">

![Zenith Workspace](https://img.shields.io/badge/Platform-Windows%2010%2F11-blue)
![Version](https://img.shields.io/badge/Version-1.0.0-brightgreen)
![License](https://img.shields.io/badge/License-Proprietary-red)

*Transform your desktop into a zen productivity powerhouse*

**🏢 Developed by [Orbis Development](https://github.com/Orbis-Development)**

</div>

---

## 🌟 What Makes Zenith Special

Zenith Workspace isn't just another productivity app—it's a complete desktop transformation that brings Windows 11's design philosophy to life with stunning glassmorphism effects and intelligent productivity tools.

### ✨ **Premium Features**

🎯 **Smart Widget Ecosystem**
- **Quick Notes** - Lightning-fast thought capture with markdown support
- **Advanced System Monitor** - Real-time performance graphs and analytics
- **Intelligent Clipboard** - Smart history with AI-powered search
- **Focus Timer** - Scientifically-designed Pomodoro sessions

🌈 **Next-Gen UI Design**
- True glassmorphism with hardware-accelerated blur effects
- Adaptive color schemes that respond to your workflow
- Fluid animations with 60fps smoothness
- Native Windows 11 integration

⚡ **Pro Productivity**
- Global shortcuts that work system-wide
- Invisible system tray mode for zero distraction
- Cross-session data persistence and analytics
- Customizable widget layouts and sizes

---

## 🚀 Download & Installation

### 💎 **Get Zenith Workspace**

**[⬇️ Download Latest Release](https://github.com/Orbis-Development/Zenith-Workspace/releases)**

Choose your installation method:
- **🔧 NSIS Installer** - Professional installation with shortcuts and uninstaller  
- **📦 Portable Version** - Run directly without installation
- **🔄 Auto-Updates** - Stay current with the latest features

### 📋 **System Requirements**
- Windows 10 (version 1903+) or Windows 11
- 4GB RAM minimum (8GB recommended) 
- 200MB free disk space
- DirectX 11 compatible graphics (for glassmorphism effects)

### ⚡ **Quick Start**
1. Download the installer from releases
2. Run `Zenith-Workspace-Setup-1.0.0.exe`
3. Follow the installation wizard
4. Launch Zenith from desktop shortcut or Start menu
5. Press `Ctrl+Shift+Z` to open the main dashboard

---

### 🌟 **Glassmorphism Design**
- Translucent, blurred backgrounds that feel native to Windows 11
- Smooth animations and micro-interactions
- Ambient focus modes with subtle color overlays
- Modern typography and iconography

### ⚡ **Productivity Features**
- Global keyboard shortcuts for instant access
- System tray integration for minimal distraction
- Auto-saving and persistent data storage
- Cross-session activity tracking

## 🚀 Quick Start

### Prerequisites
- Node.js 16+ 
- Windows 10/11 (primary target, but cross-platform compatible)

### Installation

1. **Clone and Setup**
   ```bash
   git clone <repository-url>
   cd zenith-workspace
   npm install
   ```

2. **Development Mode**
   ```bash
   npm run dev
   ```

3. **Build for Production**
   ```bash
   npm run build-win
   ```

## 🎮 Usage

### Global Shortcuts
- `Ctrl+Shift+Z` - Show/hide main window
- `Ctrl+Shift+N` - Quick note capture
- `Ctrl+Shift+M` - System monitor widget
- `Ctrl+Shift+C` - Clipboard manager
- `Ctrl+Shift+T` - Focus timer

### Focus Modes
- `Ctrl+Alt+1` - Deep Work mode
- `Ctrl+Alt+2` - Creative mode  
- `Ctrl+Alt+3` - Break time mode

### Widget Controls
- **Drag** widget headers to reposition
- **Right-click** widgets for context menus
- **Double-click** system tray icon to show main window

## 🏗️ Architecture

### Main Process (`src/main.js`)
- Window management and system integration
- Global shortcuts and tray functionality
- IPC communication with renderers
- System monitoring and stats collection

### Renderer Process (`src/renderer/`)
- Main application interface
- Dashboard and activity management
- Focus mode controls and ambient effects

### Widget Components (`src/components/`)
Each widget is a self-contained HTML file with:
- Embedded CSS for glassmorphism styling
- JavaScript for functionality and IPC
- Local storage for persistence

## 🎨 Design System

### Colors
```css
--primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
--glass-primary: rgba(255, 255, 255, 0.1);
--glass-border: rgba(255, 255, 255, 0.2);
```

### Typography
- **Font**: Inter (Google Fonts)
- **Weights**: 300, 400, 500, 600, 700
- **Hierarchy**: 48px → 20px → 14px → 12px → 10px

### Spacing System
- **xs**: 4px, **sm**: 8px, **md**: 12px-16px, **lg**: 20px-24px, **xl**: 32px+

## 🔧 Development

### Project Structure
```
zenith-workspace/
├── src/
│   ├── main.js              # Main Electron process
│   ├── renderer/            # Main window files
│   │   ├── index.html
│   │   ├── styles.css
│   │   └── renderer.js
│   └── components/          # Widget components
│       ├── quick-notes.html
│       ├── system-monitor.html
│       ├── clipboard.html
│       ├── focus-timer.html
│       └── widget-styles.css
├── assets/                  # Icons and static files
├── package.json
└── README.md
```

### Adding New Widgets

1. Create widget HTML file in `src/components/`
2. Follow the widget template structure:
   ```html
   <div class="widget-header">...</div>
   <div class="widget-content">...</div>
   <script>/* Widget logic */</script>
   ```
3. Register widget type in `src/main.js`
4. Add widget button to main interface

### Styling Guidelines
- Use CSS custom properties for theming
- Implement glassmorphism with `backdrop-filter: blur(20px)`
- Maintain consistent spacing using design tokens
- Test transparency effects on various backgrounds

## 📦 Building & Distribution

### Windows Installer
```bash
npm run build-win
```
Creates NSIS installer in `dist/` directory.

### Portable Version
The built application can run as a portable executable without installation.

### Development vs Production
- Development: Hot reload enabled, DevTools open
- Production: Optimized bundle, no DevTools, auto-updater ready

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-widget`
3. Follow the glassmorphism design system
4. Test on Windows 10 and 11
5. Submit a pull request

### Code Style
- Use Prettier for formatting
- Follow ESLint configuration
- Write self-documenting code
- Test widget interactions thoroughly

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 🙏 Acknowledgments

- **Design Inspiration**: Windows 11 Fluent Design
- **Icons**: Native emoji and Unicode symbols
- **Typography**: Google Fonts (Inter)
- **Framework**: Electron.js community

---

<div align="center">

**Built with ❤️ for productivity enthusiasts**

*Developed by Orbis Development*

---

## 📞 Support & Contact

### 🏢 **Orbis Development Team**
- 💬 **Discord:** `relationalthrone2`  
- ☕ **Ko-fi:** `xlelords`
- 📧 **Support:** `support@orbisdev.com`
- 🌐 **Website:** `https://orbisdev.com`

### 📋 **License & Distribution**
Zenith Workspace is proprietary software.  
© 2025 Orbis Development. All rights reserved.

*This software is not open source. Redistribution requires written permission.*

</div>

</div>

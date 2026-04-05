<div align="center">
  <a href="https://github.com/Liberchat/Liberchat">
    <img src="assets/icon.ico" alt="Liberchat Logo" width="96" height="96" style="margin-bottom: 10px;" />
  </a>
  
  <h1 style="margin-top: 0;">Liberchat Desktop 2.0.1</h1>
  
  <a href="https://github.com/Liberchat/Liberchat">Main project on GitHub</a>
  
  <br/>
  
  <img src="https://img.shields.io/badge/Version-2.0.1-brightgreen"/>
  <img src="https://img.shields.io/badge/Electron-22.x-blue?logo=electron"/>
  <img src="https://img.shields.io/badge/Linux-compatible-success?logo=linux"/>
  <img src="https://img.shields.io/badge/UI-Modern-red"/>
  <img src="https://img.shields.io/badge/license-MIT-green"/>
  
  <br/>
  <em>Modern messaging application with server history and customizable themes.</em>
</div>

## What's new in version 2.0.1

### Server History
- **Smart dropdown menu**: Automatically remembers your last 5 used servers
- **Quick selection**: Click on a server from the history to select it instantly
- **Easy management**: Remove unwanted servers with a single click
- **No duplicates**: Automatically prevents duplicate entries

### Theme System
- **Dark/Light mode**: Toggle between themes according to your preferences
- **Auto mode**: Automatically follows your system theme
- **Persistence**: Your preferences are saved between sessions
- **Complete interface**: All elements adapt to the chosen theme

### Smart Save
- **Persistent configuration**: History and theme are saved automatically
- **Local file**: Data is stored in `~/.liberchat/config.json`
- **Error recovery**: Robust handling of corrupted data

## Main Features
- Stylized **Splash screen** with server selection
- **Microphone compatibility** (automatic permissions)
- **Security**: contextIsolation, secure preload
- **Maximized main window, without menu bar**
- **System icon**: Correct display in the taskbar
- **Universal Linux build**: AppImage, deb, rpm

## Installation & Launch

```bash
# Install dependencies
npm install

# Run in development mode
npm start

# Generate packages for Linux (AppImage, deb, rpm)
npm run build
```

The generated files are located in the `dist/` folder.

## Installation on Linux

After compiling (`npm run build`), you will find in the `dist/` folder:

- **AppImage** (`.AppImage`): universal, executable on most distributions.
  - Make the file executable: `chmod +x Liberchat-*.AppImage`
  - Run it: `./Liberchat-*.AppImage`

- **Debian/Ubuntu** (`.deb`):
  - Install with: `sudo dpkg -i Liberchat-*.deb`
  - Or double-click the file in your file manager.


- **Red Hat/Fedora/SUSE** (`.rpm`):
  - Install with: `sudo rpm -i Liberchat-*.rpm`
  - Or double-click the file in your file manager.

> **Tip**: AppImage works on most distributions without system installation.

## Server Configuration
On startup, enter the Liberchat server URL of your choice in the splash screen.

## Main Dependencies
- [Electron](https://www.electronjs.org/) ^22.x
- [electron-builder](https://www.electron.build/)

## License
MIT

---
Modern project, designed for compatibility and ease of use on all Linux distributions.

## Usage

### Server Configuration
1. **First launch**: Enter the Liberchat server URL in the splash screen
2. **Subsequent servers**: Click in the URL field to see your server history
3. **Quick selection**: Choose a server from the dropdown list

### Customization
- **Change theme**: Click on the theme toggle icon in the top right corner
- **Manage history**: Use the close button to remove servers from history

### Default Server
The application connects by default to: `https://liberchat.cnt-ait-contact.noho.st/liberchat`

## Changelog v2.0.1
- Added server history with dropdown menu
- Dark/light/auto theme system
- Persistent saving of user preferences
- Fixed icon display in the taskbar
- Improved and more intuitive user interface


# Kill the Cockroaches – A Fun PWA Game

**Live Demo**: [Play Now](https://Palay-en.github.io/kill-the-cockroaches/)

Dive into a thrilling bug-squashing adventure! This Progressive Web App (PWA) lets you eliminate cockroaches with a slipper cursor. Fully offline-capable and installable, it’s built with pure web technologies.

---

## Overview

### Key Features

- **Instant Play**: Accessible via GitHub Pages.
- **Audio Control**: Mute or unmute background music and sound effects.
- **Game Timer**: Tracks your play session.
- **Kill Counter**: Displays the number of cockroaches squashed.
- **Offline Mode**: Works seamlessly without an internet connection.
- **Dynamic Difficulty**: Spawn rate increases every 10 seconds.
- **Custom Cursor**: Slipper-themed pointer for gameplay.
- **Immersive Audio**: Background music and squish sound effects.
- **Death Animation**: Visual feedback when cockroaches are squashed.

---

## How to Access

**URL**: [https://Palay-en.github.io/kill-the-cockroaches/](https://your-github-username.github.io/kill-the-cockroaches/)

No installation required—just open the link in your browser and start playing!

---

## Installation Guide (Optional)

1. Open the game link in a PWA-compatible browser (e.g., Chrome, Edge).
2. Look for the **Install** option in the address bar and click it.
3. The game will be added to your home screen or desktop.
4. Enjoy offline gameplay with all features intact!

---

## Gameplay Instructions

1. **Start Playing**: Click on cockroaches to squash them.
2. **Stay Alert**: The spawn rate increases every 10 seconds.
3. **Control Audio**: Use the mute/unmute button to toggle sound.
4. **Track Progress**: Check the timer and kill count at the top of the screen.
5. **Offline Play**: The game remains functional even without internet access.

---

## Technology Stack

- **HTML5**, **CSS3**, **JavaScript**
- **PWA Features**: Web app manifest and optional service worker.
- **Web Audio API**: For background music and sound effects.
- **Offline Detection**: Using `navigator.onLine`.
- **Custom Cursor Styling**: CSS-based.

---

## Project Structure

```
/
├── index.html              # Main game interface
├── manifest.json           # PWA configuration
├── assets/
│   ├── icon-192.png        # App icon (192x192)
│   ├── icon-512.png        # App icon (512x512)
│   ├── cockroach.png       # Cockroach sprite
│   ├── dead-roach.png      # Dead cockroach sprite
│   ├── slipper-cursor.png  # Custom cursor image
│   ├── music.mp3           # Background music
│   └── squish.mp3          # Sound effect for squashing
```

> **Note**: To enable offline caching, consider adding a `sw.js` service worker.

---

## Game Mechanics

- **Dynamic Spawn Rate**: Cockroach spawn rate increases every 10 seconds.
- **Click Detection**: Detects clicks on cockroaches to trigger actions.
- **Feedback System**:
  - Plays `squish.mp3` sound.
  - Replaces the sprite with `dead-roach.png`.
  - Updates the kill counter.
- **Custom Cursor**:

```css
body {
  cursor: url('./assets/slipper-cursor.png'), auto;
}
```

- **Offline Notification**:

```js
window.addEventListener('offline', () => {
  alert("You're offline. The game will still work!");
});
```

---

## Planned Features

- Mobile touch support.
- Leaderboard using localStorage or a database.
- Animated cockroach movement.
- Level progression system.
- Adjustable sound and music volume.
- Game over screen with a restart option.

---


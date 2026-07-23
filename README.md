# owl-player.github.io

A privacy-first, offline React audio player that automatically bookmarks your playback position in browser storage so you can resume listening later.

# 🎵 Offline React Audio Player

A lightweight, serverless, and privacy-focused audio player built with React and TypeScript. This application allows you to load and play audio files entirely in-memory—meaning your files are never uploaded to a server, keeping your data 100% private and secure.

### ✨ Key Features

*   **Smart Playback Resuming:** Automatically creates a unique local signature for your audio files based on file metadata. If you refresh the page or return days later, it instantly remembers exactly where you left off.
*   **100% Local Processing:** Uses HTML5 Blob URLs to stream audio directly from your RAM. Zero server costs, zero database overhead, and completely offline-capable.
*   **Custom Control Layout:** Includes custom play/pause transport controls, a responsive progress seek bar, and accurate `MM:SS` time counters.
*   **Race-Condition Safe:** Implements a strict synchronous locking mechanism via React refs to ensure your saved bookmarks are never accidentally overwritten during audio initialization.

### 🛠️ Built With

*   React
*   TypeScript
*   HTML5 Audio API + LocalStorage
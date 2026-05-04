#  Hyprealm — Browser-Based Window Manager

A keyboard-driven, floating window system inspired by Hyprland — built entirely in vanilla JavaScript.

This project recreates core window manager behaviors directly in the browser: draggable windows, snapping, animated transitions, and a minimal workflow focused on speed and control.

✨ Features
* 🤗 Draggable, resizable windows with momentum
* ⚡ Keyboard-first workflow (spawn, close, launch apps)
* 🧲 Edge snapping (left / right / fullscreen)
* 👻 Snap preview ghost (real-time visual feedback)
* 🎯 Snap-to-ghost animation (no jarring jumps)
* 🔁 Restore previous size after unsnapping
* 🧠 Lightweight task manager mock window
* 📝 Editable console windows (textarea-based)
* 🎬 Smooth open / close / focus animations

# ⌨️ Keybinds
## Key	Actions

* 'n'	Open new window
* ';'	Close active window
* 'Y Y'	Open YouTube (In quick succession)
* 'G G'	Open Google (In quick succession)
* 'tilde tilde'	Open Task Manager

## 🧠 Design Philosophy
* Keyboard-first — minimize reliance on UI buttons
* Immediate feedback — ghost previews and smooth transitions
* Minimal state, maximum feel — simple logic, polished UX
* No frameworks — everything built from scratch

## 🏗️ How It Works
Each window is a DOM element with:

- Absolute positioning
- Drag + resize handlers
- Internal state (snapped / previous bounds)
- Snapping
- Triggered on mouse release
- Uses edge detection + threshold
- Stores previous size for restoration
- Ghost Preview
- Separate overlay element
- Updates during drag
- Acts as the source of truth for snapping
- Animation Layer
-  CSS transitions for movement and scaling
- JS-controlled transitions for snapping
- Disabled during drag for responsiveness

## 🔮 Coming Soon:
* Quadrant snapping (tiling layout)
* Magnetic edge snapping
* Workspace system (virtual desktops)
* Persistent window state (localStorage)
* Terminal command parsing
* Window stacking / z-index management
* App system (YouTube, notes, etc. as windows)

## ⚠️ Limitations
* Not a real window manager (runs in browser sandbox)
* No process isolation
* No true multi-monitor awareness
* Performance tied to DOM rendering

## 🤝 End Notes
This is a personal experimental project, but feel free to fork and build on it.
This project is less about replicating an OS and more about understanding why modern window managers feel the way they do.
Turns out — it's mostly good state management and even better animations.

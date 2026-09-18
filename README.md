# Mind Mesh 🧠🌐
> **Created by HattyHats**  
> A zero-backend, 100% in-browser, cryptographic spatial mind-mapping workspace.

---

## Overview ✨

**Mind Mesh** is a privacy-first, spatial idea sandbox designed to think the way your brain thinks: organically, visually, and without limits. 

Unlike traditional cloud note-taking tools that require accounts, monthly subscriptions, and central databases storing your private notes, **Mind Mesh runs 100% locally inside your web browser**. 

- **Zero Cloud Servers**: No accounts, no logins, no tracking, and zero telemetry.
- **Client-Side Cryptography**: Your mind map is encrypted with native `SubtleCrypto` AES-GCM 256-bit encryption.
- **Spatial Freedom**: Drag, connect, cluster, nest, and traverse your thoughts across an infinite physics-driven canvas.

---

## ⚠️ Important: Understanding the "URL Link Limit Approaching" Popup

As you build out your mind map, you might notice a yellow notification in the upper-right corner:
> **"Large map: URL link limit approaching. Save as .mesh file!"**

### Why does this happen?
To allow you to share or bookmark an entire encrypted mind map without requiring a server database, Mind Mesh encrypts your graph and places the encrypted ciphertext directly in the **URL address bar** (after the `#` hash). 

However, modern web browsers (Chrome, Safari, Firefox, Edge) place practical length limits on web addresses (around **2,000 characters**). When your mind map grows large—such as after loading the sample mind map or connecting multiple ideas—the encrypted string exceeds this 2,000-character bookmarking limit.

### Is my work safe?
**Yes, 100%!**  
Mind Mesh automatically and continuously auto-saves your entire mind map right in your browser's local storage (`localStorage`). Closing or refreshing the page will not lose your work.

### What should you do?
1. **Save to your computer**: Click the **Save** button in the top navigation bar (or the **"Save .mesh"** button directly inside the notification). This downloads a standalone `.mesh` file to your computer.
2. **Reopen anytime**: You can open that file later using the **Open** button in the top bar or simply by **dragging and dropping** your `.mesh` file directly onto the browser window.
3. **Dismiss the banner**: Click the **✕** button on the notification to close it whenever you wish.

---

## Key Features 🚀

### 1. Spatial Mind Mapping & Navigation
- **Spawn Thoughts**: Double-click anywhere on the canvas or click **+ Thought** in the top bar.
- **Link Thoughts**: Hold **Shift** and drag from one thought to another to form interconnected relational edges.
- **Lasso Multi-Select**: Hold **Shift** and drag across empty canvas space to select multiple thoughts at once.
- **Snap to Grid**: Hold **Alt** while dragging thoughts to snap them to a crisp 50px grid.
- **Cursor-Centered Zoom & Panning**: Use your mouse wheel or 2-finger trackpad pinch to zoom smoothly straight into any node.
- **WASD Navigation**: Use keyboard keys <kbd>W</kbd>, <kbd>A</kbd>, <kbd>S</kbd>, <kbd>D</kbd> to fly across large canvas networks.

### 2. 3D Particle Splash Screen
- Experience a 3D warp-speed fly-through of floating thought bubbles with interconnected neural filaments.
- Cyber-glitch typographic title sequence: **Mind Mesh** with RGB chromatic split and **Created by HattyHats** neon glitch animation.
- Replayable anytime via the top right menu (`...` > *Replay Intro Splash*).

### 3. Interactive Slash Commands (`/`)
When typing a thought title or note, type `/` to bring up the interactive command palette:
- `/brainstorm [topic]` - Automatically spawn 3 connected sub-ideas.
- `/cluster` - Group related ideas into organized glassmorphic boxes.
- `/box [Name]` - Create a spatial container box for categorizing thoughts.
- `/embed [URL]` - Embed live interactive YouTube videos or web pages directly inside a thought.
- `/lock [Secret]` - Encrypt individual thoughts with your master vault password.
- `[[Wikilinks]]` - Automatically link thoughts together by category tag.
- Color tags: `/red`, `/blue`, `/green`, `/purple`, `/amber`.

### 4. 3-Tier Hybrid AI Engine
- **Tier 1: Instant Offline Heuristic AI (Default)**: Zero-latency, 100% reliable concept ideation, serendipity linking, and semantic clustering without downloading heavy models or requiring a GPU.
- **Tier 2: WebGPU Web-LLM (Optional)**: Deep local Llama 3.2 execution running entirely on your machine's WebGPU.
- **Tier 3: Cloud API (Optional)**: Connect your Google Gemini or OpenAI API key in Settings for cloud-powered models.

### 5. Master Vault & Decentralized Security
- **AES-GCM Encryption**: PBKDF2 key derivation with 100,000 rounds.
- **Thought Vaults**: Lock sensitive ideas behind a master password.
- **Panic Burn**: Instant cryptographic wipe of graph state from memory.
- **Incognito Mode**: Automatically wipes memory if you switch tabs or blur the browser window.

### 6. Timeline Calendar & History
- Automatic timestamping of every idea.
- Navigate months with `<` and `>` to filter and trace the chronological evolution of your thinking.
- Timeline slider to scrub through the history of how your mind map was constructed over time.

### 7. Universal Exports
- **`.mesh` File**: Native JSON graph export with encryption metadata.
- **Markdown (`.md`)**: Export your ideas as clean, readable Markdown documents.
- **Obsidian Vault (`.zip`)**: Export directly into an Obsidian-compatible folder structure with bidirectional wikilinks.
- **Steganography (`.png`)**: Hide and embed your entire encrypted mind map invisibly inside a standard PNG image!

---

## Quick Start 💻

### Running Locally
1. Clone the repository and install dependencies:
   ```bash
   git clone https://github.com/HattyHats/Neural-Mesh.git
   cd Neural-Mesh
   npm install
   ```

2. Start the local development server:
   ```bash
   npm run dev
   ```
   *Your default browser will automatically open `http://localhost:5173`.*

3. Build for production:
   ```bash
   npm run build
   ```
   *Generates high-performance, statically hostable assets in the `dist/` directory ready for GitHub Pages, Netlify, Vercel, or cloud storage.*

---

## Keyboard Shortcuts & Gestures ⌨️

| Action | Shortcut / Gesture |
| :--- | :--- |
| **Spawn Thought** | Double-Click on canvas or click `+ Thought` |
| **Slash Commands** | Type `/` inside thought input |
| **Connect Thoughts** | <kbd>Shift</kbd> + Drag from thought to thought |
| **Lasso Multi-Select** | <kbd>Shift</kbd> + Drag on empty canvas space |
| **Grid Snap** | Hold <kbd>Alt</kbd> while dragging node |
| **Search & Teleport** | <kbd>Cmd</kbd> + <kbd>K</kbd> (or <kbd>Ctrl</kbd> + <kbd>K</kbd>) |
| **Quick Thought Dump Inbox** | <kbd>Alt</kbd> + <kbd>N</kbd> or <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>Space</kbd> |
| **Undo / Redo** | <kbd>Cmd/Ctrl</kbd> + <kbd>Z</kbd> / <kbd>Cmd/Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Z</kbd> |
| **Pan Canvas** | 2-Finger scroll / trackpad drag |
| **Zoom In / Out** | Pinch gesture or <kbd>Cmd/Ctrl</kbd> + Mouse Wheel |
| **Collapse / Expand Branch** | Right-Click any Category or Date node |
| **Delete Selected Thought** | <kbd>Backspace</kbd> or <kbd>Delete</kbd> |

---

## Credits & License 📜

- **Creator**: Created by **HattyHats**
- **License**: MIT License


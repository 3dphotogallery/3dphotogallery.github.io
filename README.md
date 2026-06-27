# 3D Photo Gallery 🖼️

An interactive 3D photo gallery featuring a rotating carousel with stunning 3D effects, mirror reflections, and automatic daily photo updates. Built with pure HTML, CSS, and JavaScript — no frameworks or dependencies.

## 🔗 Links

- **Live Application:** [https://3dphotogallery.github.io](https://3dphotogallery.github.io)

## ✨ Features

- **3D Rotating Carousel** — Photos arranged in a circular 3D ring with smooth rotation animations and depth-based opacity fading.
- **Mirror Reflections** — Realistic reflection effect beneath each photo (toggleable).
- **Two Photo Sources** — Choose between different external image providers, instantly regenerating the gallery.
- **Automatic Daily Updates** — Fresh photos load automatically once per day; a background timer refreshes the gallery if it stays open past midnight.
- **Manual Refresh** — Force-load new photos anytime with the refresh button.
- **Dual Orientation** — Switch between horizontal (Y-axis) and vertical (X-axis) carousel rotation.
- **Bilingual Support** — Ukrainian (default) and English, covering all UI text and captions.
- **Persistent State** — Language, orientation, reflection setting, current photo, source, photo set, and last update time are saved to `localStorage` and restored on reload.
- **Fullscreen Viewer** — Tap the active photo to open a high-resolution modal view.
- **Auto-Rotate Mode** — Hands-free automatic slideshow.
- **Fully Responsive** — Adaptive sizing, dynamic 3D radius, safe-area support, and optimized layouts for small screens and landscape orientation.
- **Touch & Keyboard Controls** — Swipe gestures, arrow key navigation, and click/tap interactions.

## 🚀 Getting Started

Since this is a single, self-contained HTML file with no build step or dependencies, you can run it instantly. Simply open the `index.html` file in your web browser.

## 🎮 Usage

| Control | Action |
|---------|--------|
| **‹ / ›** buttons | Navigate to previous / next photo |
| **Arrow keys** | Navigate the carousel |
| **Swipe** | Browse photos on touch devices |
| **Tap active photo** | Open fullscreen viewer |
| **🔄 Orientation** | Toggle horizontal / vertical rotation |
| **🌐 Language** | Switch between Ukrainian and English |
| **✨ Reflection** | Toggle the mirror reflection effect |
| **▶ Auto** | Start / stop auto-rotate slideshow |
| **Photo source** | Select the external image provider |
| **⬇ Refresh photos** | Manually load a new set of photos |
| **Esc** | Close the fullscreen viewer |

## 🛠️ Technical Details

- **Zero dependencies** — Pure vanilla HTML, CSS, and JavaScript.
- **Single file** — Everything (markup, styles, scripts, and an inline SVG favicon) lives in one `index.html`.
- **CSS 3D Transforms** — Uses `perspective`, `transform-style: preserve-3d`, and `rotateX/rotateY` for the 3D effects.
- **Responsive radius** — The carousel radius is calculated dynamically from card dimensions and clamped to the viewport, so cards never overflow on small screens.
- **External image sources** — Keyless public image services are used by default. To integrate API-based providers (e.g., with keys), replace the `thumb`/`full` functions in the `SOURCES` object and store the returned URLs in `state.photos`.

## 📄 License

MIT

# 🧮 Calculator by f0undr
> **Precision Meets Innovation** — High-precision scientific calculator, memory registers, calculation history vault, and multi-category unit converter. Fully optimized for Mobile and Desktop PC.

---

## 📱 Mobile Optimizations

- **Native Touch Ergonomics**:
  - `touch-action: manipulation` eliminates the 300ms mobile double-tap latency and accidental pinch-zoom on keys.
  - Haptic feedback (`navigator.vibrate`) on supported Android and mobile browsers for tactile physical feedback.
  - `-webkit-tap-highlight-color: transparent` with immediate active key-press state.
  - Safe-area padding (`env(safe-area-inset-*)`) ensures proper display on notch screens and home indicator bars (iPhone / Android).
- **Mobile Bottom Sheet for History**:
  - Tapping `⟲` smoothly slides up an iOS/Android-style bottom sheet modal with backdrop blur and drag handle.
- **Landscape Mode**:
  - Automatic adaptation to landscape orientation (`@media (orientation: landscape)`): compresses header, aligns scientific and standard pads side-by-side, fitting completely within the screen height with zero scrolling.
- **Mobile Number Keypad**:
  - All converter inputs utilize `inputmode="decimal"` to invoke the native mobile decimal keyboard instead of the alphanumeric keyboard.

---

## 💻 PC & Desktop Optimizations

- **Full Physical NumPad Support**:
  - Complete support for `Numpad0`–`Numpad9`, `NumpadAdd` (`+`), `NumpadSubtract` (`-`), `NumpadMultiply` (`×`), `NumpadDivide` (`÷`), `NumpadDecimal` (`.`), and `NumpadEnter` (`=`).
- **Clipboard Integration**:
  - **Copy**: Press <kbd>Ctrl</kbd> + <kbd>C</kbd> (or <kbd>Cmd</kbd> + <kbd>C</kbd>) to instantly copy the current calculation to clipboard.
  - **Paste**: Press <kbd>Ctrl</kbd> + <kbd>V</kbd> to paste equations or numbers straight into the calculator.
- **Desktop Keyboard Shortcuts**:
  - <kbd>H</kbd>: Toggle History sidebar
  - <kbd>T</kbd>: Toggle Light / Dark theme
  - <kbd>D</kbd>: Toggle Angle Mode (DEG / RAD)
  - <kbd>M</kbd>: Add current value to memory (<kbd>M+</kbd>)
  - <kbd>Esc</kbd> / <kbd>Delete</kbd>: Clear All (<kbd>AC</kbd>)
  - <kbd>Backspace</kbd>: Backspace
  - <kbd>s</kbd> / <kbd>c</kbd> / <kbd>t</kbd>: `sin(`, `cos(`, `tan(`
  - <kbd>l</kbd>: `log(`
  - <kbd>p</kbd> / <kbd>e</kbd>: `π` / `e`
  - <kbd>!</kbd> / <kbd>^</kbd>: Factorial / Exponent
- **Responsive Large Screen Dashboard**:
  - Fluid typography scaling via CSS `clamp()` and responsive grid system that adapts smoothly from 320px phones to 4K monitors.
  - Custom scrollbars styled to blend with dark and light themes.

---

## ✨ Core Features

- **Standard Mode**: Clean 4-column layout for fast arithmetic.
- **Scientific Mode**:
  - Trigonometric: `sin`, `cos`, `tan`, `sin⁻¹`, `cos⁻¹`, `tan⁻¹`
  - Hyperbolic: `sinh`, `cosh`, `tanh`
  - Powers & Roots: `x²`, `x³`, `xʸ`, `√x`, `³√x`, `10ˣ`, `eˣ`, `2ˣ`
  - Logarithms: `log₁₀`, `ln`, `log₂`
  - Factorials: `n!`
  - Constants: `π`, `e`
  - Angle Modes: Seamless `DEG` / `RAD` toggle
  - `2nd` Shift Mode: Flips between standard and secondary inverse functions.
- **Multi-Category Unit Converter**:
  - Instant bi-directional conversion across **8 categories**: Length, Mass, Temperature, Digital Storage, Speed, Time, Area, Volume.
  - **"Send to Calculator"** button to pipe any converted number back into equations.
- **Memory System (MC, MR, M+, M-, MS)**:
  - Registers persist in `localStorage` with active badge indicators.
- **History Vault & Export**:
  - Time-stamped calculations with one-click reload.
  - Export calculation history as `.csv`.
- **Sensory & Visual Polish**:
  - Web Audio API synthesizer for tactile mechanical click sounds (`🔊`/`🔇` toggle).
  - Floating toast notifications.
  - PWA ready (`manifest.json` + `icon.svg`).

---

## 🚀 How to Run

Open [`index.html`](./index.html) in any modern browser (Chrome, Edge, Safari, Firefox).

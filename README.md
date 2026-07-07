# 🌙 Eid Salami Wheel

An interactive, responsive, and visually stunning web-based **Eid Salami Lucky Wheel** built using HTML5 Canvas, modern CSS variables, and JavaScript. Featuring a premium **Islamic Golden Theme**, fluid animations, and celebratory confetti effects, it adds a touch of digital joy to Eid celebrations.

---

## 🚀 Live Demo

Try out the live web application here:  
👉 **[https://salami-wheel.netlify.app/](https://salami-wheel.netlify.app/)**

---

## ✨ Features

- **🏆 Ornate Golden Theme:** Styled with an elegant palette including emerald green, crimson red, and metallic gold accents, driven by custom CSS variables (`:root`).
- **🎯 Dynamic Canvas Wheel:** Dynamically renders text and slices from an array of randomized monetary amounts (ranging from `0.25 Tk` to `10.00 Tk`) using the HTML5 Canvas API.
- **📱 Fully Responsive Layout:** Employs modern CSS techniques like `clamp()`, `aspect-ratio: 1 / 1`, and standard view units (`vw`) to ensure a flawless presentation across all desktop, tablet, and mobile displays.
- **♾️ Infinite Spins:** Allows users to spin the wheel multiple times sequentially without blockades, instantly resetting the button state back to active after each round.
- **🎉 Immersive Celebrations:** Integrates `canvas-confetti` to trigger custom gold and silver cascading confetti showers once the wheel lands on a prize.

---

## 🛠 Tech Stack

- **Markup:** HTML5
- **Styling:** CSS3 (Custom Properties, SVG Background Patterns, Fluid Typography)
- **Typography:** Google Fonts (`Amiri`)
- **Scripting:** Pure Vanilla JavaScript (ES6+)
- **Libraries:** [Canvas Confetti](https://github.com/catdad/canvas-confetti) (Loaded via CDN)

---

## 📂 File Structure

```text
├── Salami_Wheel.html   # Main application file containing structure, styling, and logic
└── README.md           # Repository documentation

```

---

## 🛠 How to Run Locally

Since the project is completely self-contained within a single HTML file, getting it running is fast and effortless:

1. **Clone the repository:**
```bash
git clone [https://github.com/SarafatAlamIrfan/eid-salami-wheel.git](https://github.com/SarafatAlamIrfan/eid-salami-wheel.git)

```


2. **Navigate into the directory:**
```bash
cd eid-salami-wheel

```


3. **Open the file:**
Simply double-click `Salami_Wheel.html` to run it directly in any modern web browser.

---

## ⚙️ How It Works

1. **Generation & Shuffle:** On load, JavaScript dynamically populates an options array with increments of `0.25 Tk` up to `10.00 Tk`, then shuffles them using a Fisher-Yates randomization technique before drawing slices onto the high-resolution canvas.
2. **Physics Simulation:** Clicking "Spin the Wheel" computes a combination of deterministic rotations (multiple full $360^\circ$ spins) plus a randomized remainder degree, governed by a fluid `cubic-bezier` CSS transition curve lasting 4 seconds.
3. **Angle Decryption:** When the transition stops, the absolute degree offset is checked against the mathematical arc size per slice to identify the absolute winning tier, which is subsequently shown inside a crisp modal window.

---

## 📜 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE).

---

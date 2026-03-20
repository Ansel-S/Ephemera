# ⏳ Ephemera

**A minimalist, intentional reading queue that encourages focus through decay.**

Ephemera is a lightweight tool designed to solve "tab debt." It strips away the clutter of traditional "read-it-later" apps, forcing you to prioritize what truly matters by limiting your queue and visualizing the passage of time.

[Live Demo](https://ansel-s.github.io/ephemera/)

---

## ✨ Key Features

- 🛑 **Hard Capacity:** A strict 10-slot limit prevents mindless hoarding and forces intentional consumption.
- 🍂 **Visual Decay:** Items transition through four stages (Fresh, Aging, Stale, Rotting) based on their age, signaling urgency.
- ⌨️ **Keyboard-First Workflow:** Rapid navigation with number keys (1-9), quick-delete (Shift + Num), and instant focus (`/` or `i`).
- 🔒 **Privacy by Default:** Zero tracking, zero accounts, and zero database—your data never leaves your browser's LocalStorage.
- 📱 **Serene UI:** A paper-like, responsive interface built with Lora and Inter typography for a distraction-free experience.

---

## 🛠️ The Tech Stack

- **Vanilla JavaScript:** High-performance, zero-dependency logic for state management and DOM manipulation.
- **CSS3 Variable System:** A robust system of custom properties for managing the "decay" color palette and responsive layout.
- **URL Auto-Parsing:** Intelligent link detection that automatically extracts hostnames and titles for a clean, metadata-rich list.
- **Modular Deployment:** Optimized for modern CI/CD pipelines (Vite/GitHub Actions) to bundle logic into a single-file production build.

---

## 🚀 Quick Start

### 1. Development
Clone the repo and start the local dev server:
```bash
npm install
npm run dev
```

### 2. Build
Generate the optimized single-file `index.html`:
```bash
npm run build
```

---

## 📜 License

This project is licensed under the [**MIT License**](LICENSE).

---

> 🌿 Stay intentional. Stop hoarding, start reading.

Built with ❤️ by Ansel.

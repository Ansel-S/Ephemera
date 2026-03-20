# Contributing to Ephemera

Ephemera is fully open to contributions of all kinds. Whether you found a bug, have an idea, or want to improve the code, you're welcome here — no prior experience with open source required.

---

## Reporting Bugs

Open a [GitHub issue](https://github.com/Ansel-S/Ephemera/issues/new) and include:

- What you expected to happen
- What actually happened
- Steps to reproduce
- Browser, OS, and screen size (Ephemera is a browser tool, so environment matters)

---

## Suggesting Features

Before building anything, open an issue to describe the problem you're trying to solve. A good feature suggestion explains *why*, not just *what*.

Keep Ephemera's core constraint in mind: **the 10-slot limit is a feature, not a bug.** Suggestions that route around it — unlimited slots, cloud sync, bulk import — are unlikely to be accepted, as they undermine the tool's philosophy.

---

## Submitting Code

### Setup

```bash
git clone https://github.com/Ansel-S/ephemera.git
cd ephemera
npm install
npm run dev
```

The dev server runs at `http://localhost:5173`. The production build outputs a single self-contained `index.html`:

```bash
npm run build
# Output: dist/index.html
```

### Workflow

1. Fork the repo and create a branch: `git checkout -b fix/your-description`
2. Make your changes. Keep commits small and focused.
3. Test in multiple browsers — Chrome, Firefox, and Safari if possible.
4. Open a pull request with a clear description of what changed and why.

### Code style

- **Vanilla JavaScript** for logic — no frameworks, no unnecessary dependencies.
- Lean on **CSS custom properties** for theming and the decay color palette.
- Keep the production output as a **single `index.html`** — no external assets.
- Respect the existing naming conventions and file structure.
- If you're touching the decay logic (Fresh → Aging → Stale → Rotting), make sure the timing thresholds remain intentional — they're calibrated to create a sense of urgency without feeling punishing.

### What we won't accept

- Features that remove or work around the 10-item capacity limit
- Cloud sync, accounts, or any server-side component
- External runtime dependencies that increase the bundle size significantly
- UI changes that make the tool feel busier or more anxious — Ephemera should stay calm

---

## Not Sure Where to Start?

Look for issues labeled `good first issue` or `help wanted`. Small fixes — typos, accessibility improvements, minor UI polish — are always welcome and a great way to get familiar with the codebase.

---

## Philosophy

Ephemera exists to push back against accumulation. Every contribution should serve that goal: help people read more and hoard less. When a proposed change makes the tool more powerful at the cost of making it more cluttered, the answer is probably no.

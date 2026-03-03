# 🕹️ Neon Block Blast

**Neon Block Blast** is a high-performance, mobile-responsive puzzle game built with pure Vanilla JavaScript. It combines the spatial logic of classic block puzzles with a vibrant, synth-wave neon aesthetic.

---

## 📖 Gameplay Instructions

### The Goal
Clear as many rows and columns as possible to achieve the highest score. The game ends when no more shapes from your current hand can fit anywhere on the grid.

### How to Play
* **Drag and Drop:** Grab one of the three shapes from the bottom dock and move it onto the **8x8 grid**.
* **Ghost Preview:** A semi-transparent "ghost" will appear on the grid to show exactly where the blocks will snap before you release them.
* **Clear Lines:** Fill an entire horizontal row or vertical column (8 cells) to make it flash and disappear.
* **The Shape Cycle:** You must place all **three** shapes in your dock before a new set of three is generated.
* **No Gravity:** Blocks stay exactly where you place them; clearing a line does not cause the blocks above it to fall.

### Scoring & Strategy
* **Placement:** You earn points for every individual block placed on the board.
* **Combos:** Clearing multiple lines at once triggers a **Quadratic Multiplier**:
    $$Score = (\text{Total Lines Cleared}^2 \times 10)$$
* **Pro Tip:** Keep the center of the board clear, as being forced to the edges makes it harder to fit large shapes.

---

## 🛠️ Technical Details

### Features
* **Mobile-Optimized Dragging:** Includes a vertical **touch-offset** so your finger doesn't obscure the shape while playing on a smartphone.
* **Intelligent Game-Over Detection:** Uses a "look-ahead" algorithm after every move to verify if any remaining shapes can fit in any available grid coordinate.
* **Synthesized Audio:** Uses the **Web Audio API** to generate retro-style sound effects without needing external MP3 files.

### Tech Stack
* **Language:** JavaScript (ES6+), HTML5, CSS3.
* **Layout:** CSS Grid for the 8x8 matrix and Flexbox for the UI.
* **Hosting:** Optimized for instant deployment via **Vercel**.

---

## 📂 Project Structure
```text
BLOCK-BLAST/
├── index.html      # Main entry point (HTML, CSS, and JS)
├── README.md       # Project documentation
└── daha/           # Archive/Regional folder

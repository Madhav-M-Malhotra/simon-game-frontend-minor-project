## Simon Game

Interactive, browser-based remake of the classic Simon memory game built with vanilla JavaScript, CSS, and HTML.

### 🚀 Live Demo
[Play the game](https://madhav-m-malhotra.github.io/simon-game-frontend-minor-project/) right in your browser.

### 📚 Background
Built as part of the Apna College Delta course. Independently implemented beyond the course walkthrough — includes custom styling and a simplified JavaScript approach that uses a single sequence with on‑the‑fly validation.

### 🔁 Differences from course version
- Custom styling for layout, colors, and play icon placement
- Single sequence with on‑the‑fly validation (no extra arrays for user input)
- Session high score display and logic in UI
- Input guarding by attaching/removing listeners on game start/end
- Streamlined state: minimal variables and early returns for clarity

### ✨ Features
- **Classic gameplay**: Memorize and repeat the growing color sequence.
- **Progressive difficulty**: Each round adds one more step to the sequence.
- **High score tracking**: Tracks your best run for the current session.
- **Crisp UI**: Clean layout with clear visual feedback on button flashes.
- **No build step**: Pure HTML/CSS/JS — open and play.

### 🕹️ How to Play
1. **Click the play icon** to start a new game.
2. Watch the button that flashes — that’s the first step in the sequence.
3. **Repeat the sequence** by clicking the colored buttons in order.
4. Each level adds one more step. **Miss a step and the game ends.**
5. Your highest level achieved is displayed as the **High Score** (resets on refresh).

### 🧰 Tech Stack
- **HTML5** for structure
- **CSS3** for styling
- **Vanilla JavaScript** for game logic
- **Font Awesome** (CDN) for the play icon

### 🧠 Implementation Notes
- **Single sequence array**: Uses one growing array for the game sequence and a single index (`userSeq`) to verify user input on the fly — no additional arrays; only one index for progress tracking.
- **Immediate validation**: Each click is validated as it happens; when the user completes the current sequence, the next level triggers automatically.
- **Session high score**: Tracks high score for the current session and updates UI when a new best is reached.
- **Input guarding**: Adds/removes event listeners to prevent stray input when the game is over.
- **Lightweight animations**: A simple `.flash` CSS class provides clear visual feedback.

### 📦 Project Structure
```
.
├─ index.html      # Markup and CDN includes
├─ style.css       # Styles for layout, colors, animations
├─ app.js          # Core game logic and interactions
├─ LICENSE         # MIT License
└─ README.md       # Project documentation
```

### 🖥️ Run Locally
- Option A: **Double-click** `index.html` to open in your browser.
- Option B: Serve locally (recommended):
  - With Python: `python -m http.server 5500` and visit `http://localhost:5500`
  - With VS Code: use the "Live Server" extension

### 🗺️ Roadmap / Ideas
- Add sound effects for each color press
- Add difficulty modes (speed up as levels increase)
- Persist high score using `localStorage`
- Add accessibility improvements (ARIA roles, keyboard support)

### 📜 License
This project is licensed under the **MIT License** — see [`LICENSE`](./LICENSE) for details.

### 🙌 Acknowledgements
- Built during the Apna College Delta course
- Inspired by the original Simon electronic game
- Icons by Font Awesome

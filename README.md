# THE NEXT LEVEL — KamiLimu Effect Escape Room

An interactive, third-person 3D escape-room adventure built as a creative storytelling experience for my **KamiLimu Peer Mentorship** task. Rather than presenting a traditional slideshow, this game invites the audience to walk through five interconnected rooms—solving puzzles, uncovering memories, and experiencing what **KamiLimu** means to me.

---

## Why I Built This

I created **THE NEXT LEVEL** for my **KamiLimu Peer Mentorship** presentation with two core goals:

1. **Reflecting on Professional Development Feedback:** Examining feedback from the Professional Development Competition, recognizing personal strengths and growth areas, and turning those insights into practical commitments for future applications.
2. **Showcasing the KamiLimu Effect Creatively:** Bringing to life how KamiLimu shaped my confidence, technical curiosity, problem-solving mindset, community relationships, and sense of belonging—culminating in the realization:
   > *"Because of KamiLimu, I see my potential and I am acting on it. I see growth. I have found a safe space and community. I belong."*

---

## Gameplay & The Five Rooms

Players control a custom 3D character and explore five physically connected rooms, collecting keys, inspecting photographs, and recovering five memory fragments:

1. **Room 1 — The Beginning:** Waking up in a sunlit study room to uncover early self-doubt and reconstruct the memory: *"I thought technology wasn't meant for me."*
2. **Room 2 — The Awakening:** Stepping into a responsible computing lab to shift from simply asking *"Does the code run?"* to *"Why did we choose this approach instead of another?"*
3. **Room 3 — The People:** Exploring a communal library filled with keepsake tables and photographs honoring fellow mentees, the Data Science track, ICT mentors, my peer mentor, the current Fellow, and the wider KamiLimu community.
4. **Room 4 — The Growth Room:** Reviewing evidence of personal and professional growth—including developing **ReCover**, applying for opportunities, delivering a speech (witnessed by my mum outside the programme), and logging mentor feedback reflections.
5. **Room 5 — The Future:** Uniting all four recovered memory fragments on the final pedestals to unlock the central KamiLimu reflection and a personal letter to my future self.

---

## Controls

- **`W A S D` / `Arrow Keys`** — Move character
- **`Mouse Drag`** — Orbit camera
- **`E` / `Space`** — Interact with objects, keepsakes, terminals & doors
- **`Shift`** — Sprint
- **`H`** — Request a progressive clue
- **`ESC`** — Open Pause Menu & Presenter Room Jump

---

## Technologies Used

- **HTML5 & Vanilla JavaScript (ES6+):** Core game state, character movement, collision detection, puzzle logic, and single-file export.
- **Three.js (WebGL):** 3D five-room environment, real-time lighting and shadows, animated doors, framed wall/tabletop displays, and articulated 3D character model.
- **HTML5 Canvas 2D API:** Procedural textures for hardwood floors, rugs, cork pinboard, and dynamic framed photographs with captions.
- **Tailwind CSS & Custom CSS:** Minimal game HUD, interactive puzzle modals, and presenter controls, styled with **Fredoka** and **Plus Jakarta Sans** typography.
- **Web Audio API:** Procedural sound effects (pickups, door swings, chimes, and finale chords) with zero external audio files.
- **Browser `localStorage` & `FileReader` API:** Saves game progress, reflections, and uploaded photographs locally.

---

## Project Structure

```text
the-next-level/
├── index.html          # Complete self-contained 3D escape room game
├── README.md           # Project overview and setup instructions
└── images/             # Photographs displayed on 3D room walls & Room 3 keepsake tables
    ├── r1-pinboard.jpg
    ├── r2-session.jpg
    ├── r3-mentees.jpg
    ├── r3-mentors.jpg
    ├── r4-recover.jpg
    ├── r4-speech.jpg
    ├── ks-mentees.jpg
    ├── ks-dstrack.jpg
    ├── ks-ict.jpg
    ├── ks-peer.jpg
    ├── ks-fellow.jpg
    └── ks-wider.jpg
```

---

## Running Locally & Deploying

Because browsers restrict WebGL textures from loading local images over `file:///`, run the project using a local HTTP server or deploy it online:

### Run Locally
```bash
# Using Python
python3 -m http.server 8000
# Then open http://localhost:8000 in your browser
```
*(Or right-click `index.html` in VS Code and select **Open with Live Server**.)*

### Deploy Online (GitHub Pages or Vercel)
1. Push `index.html`, `README.md`, and the `images/` folder to your GitHub repository.
2. Enable **GitHub Pages** (`Settings → Pages → Deploy from branch: main`) or import the repository into **Vercel** for an instant public presentation URL.

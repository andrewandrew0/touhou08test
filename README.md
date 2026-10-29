# 東方永夜抄 ～ Imperishable Night (Web Port - Stage 1)

A browser recreation of **Touhou 8: Imperishable Night** (*東方永夜抄 ~ Imperishable Night*), featuring authentic original graphics, Stage 1 gameplay, boss encounters, dialogue cut-ins, the full original GUI/HUD, interactive options, sound test music room, and mouse & keyboard controls.

Built for seamless hosting on **GitHub Pages** and direct browser play with zero setup required.

---

## 🎮 Playable Features

* **Original Graphics & Textures (82 sheets):**
  * **Border Team:** Reimu Hakurei & Yukari Yakumo player sprites, movement animations, hitboxes, and familiars.
  * **Stage 1 Boss:** Wriggle Nightbug (Firefly Youkai) sprites, attack frames, familiar circles, and spell cards.
  * **Stage 1 Background & Enemies:** Bamboo forest nocturnal backdrop, fairies, spirits, items, and projectile sheets (`etama` series).
  * **Dialogue Sequences:** Pre-boss dialogue portraits (`face_rm*`, `face_yk*`, `face_st01*`) with authentic cut-in layout.

* **Original GUI & HUD (`front.png`):**
  * Complete frame layout with HiScore & Score counters.
  * Remaining Lives (残機) and Bomb / Spell Card (ボム) star counters.
  * Power indicator (0 to 128 / MAX).
  * Graze counter with authentic graze effects and sound.
  * Time / Night Point counter with stage target quota.
  * **Human / Youkai Gauge:** Switches dynamically from -100% Human (Reimu) to +100% Youkai (Yukari) when holding Shift (Focus).
  * Boss Life Circle and bottom tracking **ENEMY** indicator.

* **All Main Menu Modes Supported:**
  * **Game Start:** Choose difficulty (Easy, Normal, Hard, Lunatic) → Border Team → Play full Stage 1 Arcade mode.
  * **Extra Start:** Play Stage 1 under Lunatic difficulty with full power!
  * **Spell Practice:** Jump directly into Wriggle Nightbug's spell cards with max power!
  * **Practice Start:** Stage 1 practice mode with 8 lives and 128 power!
  * **Replay:** Pre-loaded Lunatic Demo Replay showing a high-level playthrough of Stage 1, plus custom `.rpy` upload support.
  * **Result:** View session records and high scores.
  * **Music Room:** Sound test player featuring all 5 original Touhou 8 music tracks with descriptions and playback controls.
  * **Option:** Configure BGM Volume, SFX Volume, Player Lives, Player Bombs, and Mouse Controls.
  * **Quit:** Graceful thank you / credits screen.

* **Full Audio & SFX:** Original stage music, boss themes, and 36 authentic sound effects.

---

## 🕹️ Controls (Keyboard & Mouse)

### Keyboard Controls
| Key | Action | Description |
|---|---|---|
| **Arrow Keys** | Move / Navigate | Move character in game / Navigate menus |
| **Z** or **Enter** | Shoot / Confirm | Fire primary shots / Select in menus |
| **X** | Bomb / Cancel | Cast Spell Card (Bomb) / Go back in menus |
| **Shift** | Focus / Slow | Hold for precision movement, reveal player hitbox, and switch to Yukari (Youkai) |
| **Ctrl** | Fast-Forward | Fast-forward dialogue |
| **Esc** | Pause | Open pause menu |

### Mouse Controls
| Mouse Action | In Menu | In Game |
|---|---|---|
| **Hover** | Move cursor to hovered option | Move character smoothly toward cursor |
| **Left Click** | Select / Confirm | Fire shots continuously |
| **Right Click** | Go back / Cancel | Trigger Spell Card / Bomb |

---

## 🚀 How to Deploy to GitHub Pages (Play in Browser)

1. **Create a new repository** on GitHub (e.g. `touhou-8-stage1`).
2. **Push or upload all files** from this folder to the repository's `main` branch:
   * Keep `index.html` and `.nojekyll` in the root folder.
   * Keep `dist/`, `src/`, `assets/`, and `replays/` intact.
3. In your repository on GitHub:
   * Go to **Settings** → **Pages** (in the left sidebar).
   * Under **Build and deployment > Source**, select **Deploy from a branch**.
   * Under **Branch**, select `main` and folder `/ (root)`, then click **Save**.
4. Within about 1 minute, GitHub Pages will deploy your game at:
   `https://<your-username>.github.io/<repo-name>/`
5. Open the link on any desktop browser to play immediately!

---

## 💻 Playing Locally on Windows

1. Open this folder in Windows File Explorer.
2. Double-click **`play_local.bat`**.
3. It launches a local server and opens `http://localhost:8080/` in your default browser.

---

## 📁 Repository Structure

```
.
├── index.html              # Main HTML entry point
├── play_local.bat          # 1-click local launcher for Windows
├── .nojekyll               # Disables Jekyll processing on GitHub Pages
├── README.md               # Documentation and setup guide
├── dist/
│   └── th08.js             # Reconstructed TH08 runtime & original VM data
├── src/
│   └── th08.css            # 4:3 pixel-perfect responsive canvas stylesheet
├── replays/
│   └── demo.rpy            # Built-in Lunatic Stage 1 replay recording
└── assets/
    ├── th08-img/           # 82 original character, bullet, boss & UI sprite sheets
    ├── audio/th08/         # Original BGM tracks (.ogg)
    └── sfx/th08/           # Original sound effects (.wav)
```

---

### Credits & Disclaimer
* *Touhou Project* and *Imperishable Night (東方永夜抄)* are copyright © **Team Shanghai Alice / ZUN**.
* This web port implementation is for educational, archival, and non-commercial fan appreciation.

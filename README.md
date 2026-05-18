# ⭐ Star Wars Game

A Star Wars–themed space shooter game built as a Romanian **graduation certification project** (*atestat* — a mandatory final project presented at the end of high school in Romania) for 2025. The game is a Windows desktop application developed in **C# / .NET Framework 4.7.2** using **Windows Forms**, featuring animated sprites, enemy AI, projectile combat, a solar system simulation screen, and background music.

---

## 🎮 Gameplay Overview

The player controls a spaceship and must navigate through space, shooting enemies and avoiding asteroids. The game features multiple forms (screens):

- **Form1** — Main game screen with the space shooter mechanics
- **Form2** — Secondary screen (menu / info / solar system view)
- **Form3** — Additional screen (scoreboard / settings / outro)

### Controls

| Action | Key |
|---|---|
| Move Up | `↑` Arrow |
| Move Down | `↓` Arrow |
| Fire | `Space` |
| Pause | Pause button (UI) |
| Restart | Restart button (UI) |

---

## 🗂️ Project Structure

```
Star-Wars-game/
├── Atestat2025.sln              # Visual Studio solution file
└── Atestat2025/
    ├── Program.cs               # Entry point
    ├── Form1.cs / Form1.Designer.cs   # Main game form
    ├── Form2.cs / Form2.Designer.cs   # Secondary form
    ├── Form3.cs / Form3.Designer.cs   # Third form
    ├── StarWars.mdf             # SQL Server database (scores / data)
    ├── StarWars_log.ldf         # Database log file
    ├── App.config               # Application configuration
    └── bin/Debug/               # Build output & assets
        ├── Atestat2025.exe      # Compiled executable
        ├── Star Wars.mp3        # Background music
        ├── navaUp/Down/Stop/Fire/Move.png  # Player ship sprites
        ├── inamic.gif           # Enemy sprite
        ├── rachetaNava.png      # Player projectile
        ├── rachetaInamic.png    # Enemy projectile
        ├── asteroid.png         # Asteroid obstacle
        ├── forta.png            # Power-up / Force icon
        ├── Back.png             # Space background
        ├── Pamant.png           # Earth asset
        ├── luna.png             # Moon asset
        ├── Soarewatermarked.png # Sun asset
        └── ...                  # Additional character & UI assets
```

---

## 🛠️ Tech Stack

| Technology | Details |
|---|---|
| Language | C# |
| Framework | .NET Framework 4.7.2 |
| UI | Windows Forms (WinForms) |
| Database | SQL Server LocalDB (`.mdf`) |
| Audio | Windows Media Player ActiveX (`AxInterop.WMPLib`) |
| IDE | Visual Studio 2022 (recommended) |

---

## ⚙️ Prerequisites

- **Windows OS** (Windows 10 or later recommended)
- **Visual Studio 2019 / 2022** with the `.NET desktop development` workload
- **.NET Framework 4.7.2** runtime installed
- **SQL Server LocalDB** (included with Visual Studio)

---

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/iuliaaacarp/Star-Wars-game.git
   cd Star-Wars-game
   ```

2. **Open the solution**
   - Open `Atestat2025.sln` in Visual Studio

3. **Restore dependencies**
   - The project uses `AxInterop.WMPLib.dll` and `Interop.WMPLib.dll` located in `bin/Debug/`
   - These are already included in the repository — no NuGet restore needed

4. **Build and run**
   - Press `F5` or click **Start** in Visual Studio
   - Alternatively, run `Atestat2025/bin/Debug/Atestat2025.exe` directly

> **Note:** The game assets (images, GIFs, MP3, database files) must remain in the same directory as the `.exe` for the game to function correctly.

---

## 🗄️ Database

The project uses a SQL Server `.mdf` database file (`StarWars.mdf`) to store game data (e.g., scores). It is configured to copy to the output directory automatically on build. SQL Server LocalDB must be available on the machine for database functionality to work.

---

## 🎨 Assets

The game includes a rich set of visual and audio assets:

- **Player sprites:** multiple states — idle (`navaStop`), moving (`navaMove`/`navaUp`/`navaDown`), firing (`navaFire`)
- **Enemy sprites:** animated GIF enemy (`inamic.gif`) and enemy spaceship (`almir-sharifullin-1st-spaceship.gif`)
- **Environment:** space background, Sun (`Soarewatermarked.png`), Earth (`Pamant.png`), Moon (`luna.png`), asteroids
- **Characters:** Luke Skywalker, Darth Sidious / Emperor Palpatine, Star Destroyer imagery
- **Audio:** Star Wars theme music played via Windows Media Player
- **UI buttons:** Start, Pause (`Pauza.png`), Stop, Restart icons

---

## 👤 Author

Developed by **[@iuliaaacarp](https://github.com/iuliaaacarp)** as a 2025 Romanian high-school graduation certification project.

---

## 📄 License

This project is an educational assignment. Star Wars characters, names, and imagery are trademarks of **Lucasfilm Ltd. / The Walt Disney Company** and are used here for non-commercial, educational purposes only.

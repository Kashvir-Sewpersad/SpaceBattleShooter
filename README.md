# Space Battle Shooter

A simple, classic-style **space shooter** game made in **C# WPF** as a learning / portfolio project.

Pilot your spaceship, shoot enemy waves, avoid/destroy incoming threats, and try to survive as long as possible while racking up points.





![SPACE SHOOTER GIF](https://github.com/user-attachments/assets/5647625a-011c-45bf-a9bc-98552fce49ec)


## Table of Contents

- [Project Overview](#project-overview)
- [Key Features](#key-features)
- [Technologies & Approach](#technologies--approach)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
- [How to Play](#how-to-play)
- [Controls](#controls)
- [Important Notes](#important-notes)

## Project Overview

This is a lightweight, educational **2D space shooter** built with WPF.

You control a player ship at the bottom of the screen, firing bullets upward while dodging or destroying enemy ships and obstacles coming from the top.  
The project demonstrates clean game loop implementation, collision detection, sprite handling, input processing, and WPF rendering techniques using XAML + code-behind.

## Key Features

- Smooth player ship movement (left/right)
- Projectile shooting (spacebar)
- Multiple enemy types spawning in waves
- Score system based on destroyed enemies
- Collision detection (player ↔ enemy, projectile ↔ enemy, player ↔ projectile)
- Simple health / lives system (or game over on contact)
- Clean sprite/image-based rendering using WPF Image controls
- Game restart functionality

## Technologies & Approach

**Core Language & Framework**  
- C#  
- .NET WPF (.NET 6.0 / 7.0 / 8.0)

**Main Techniques & Structures**  
- **Timer** → main game loop  
- **List<T>** → active enemies, projectiles  
- **Rect** / bounding box checks → collision detection  
- **Image** controls + Canvas → rendering moving objects  
- **KeyDown / KeyUp** events → responsive input handling  
- **XAML** for UI layout + game canvas  
- Resource images stored in `/images` folder  

These choices keep the project simple, understandable, and performant for a small-scale arcade game.

## Prerequisites

- **Operating System**: Windows 10 / 11  
- **.NET SDK / Runtime**: .NET 6.0 / .NET 7.0 / .NET 8.0  
  → [Download here](https://dotnet.microsoft.com/download)  
- **IDE** (recommended):  
  - Visual Studio 2022  
  - JetBrains Rider  

## Setup Instructions

### Option 1: Clone from GitHub

1. Copy the repository URL  
   `https://github.com/Kashvir-Sewpersad/SpaceBattleShooter.git`
2. In your IDE:  
   - Visual Studio → File → Clone Repository…  
   - Rider → VCS → Get from Version Control…
3. Paste URL and clone

### Option 2: Download ZIP

1. Download ZIP from GitHub  
2. Extract to a folder (e.g. `C:\Projects\SpaceBattleShooter`)  
3. Open the `.sln` file in Visual Studio / Rider

### Run the Project

1. Open the solution (`SpaceBattleShooter.sln`)  
2. Right-click the solution → **Restore NuGet Packages** (if needed)  
3. Set the project `SpaceBattleShooter` as **Startup Project**  
4. Press **F5** or click **Run**  

The game window should launch immediately.

## How to Play

- Move your ship left/right to dodge enemies  
- Shoot projectiles to destroy incoming enemies  
- Survive as long as possible — every enemy destroyed gives points  
- Game ends when an enemy reaches you or you run out of lives/health  

Try to beat your high score!

## Controls

| Key          | Action                  |
|--------------|-------------------------|
| ← →          | Move ship left/right    |
| Space        | Fire projectile         |
| R            | Restart game            |
| Esc          | Exit / Pause            |

## Important Notes

- No external NuGet packages or APIs are used  
- All assets (sprites) are stored in the `images/` folder  
- Collision detection uses simple rectangle intersection — fast & reliable  
- Direction / movement is intentionally kept simple for learning purposes  
- AI was **not** used to write the core game logic, loop, or rendering — manually designed, coded, and tested.

---

© Kashvir Sewpersad 2025/2026  
https://github.com/Kashvir-Sewpersad/SpaceBattleShooter

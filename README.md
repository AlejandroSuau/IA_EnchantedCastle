# 🏰 Enchanted Castle — Game AI Simulation

A 3D game AI simulation developed in **Unity 6** as part of a university Master's coursework project.

Set in an enchanted castle courtyard, the project explores autonomous agent movement, navigation, perception, and decision-making using **Unity Visual Scripting**.

## 🎬 Demo

[![Watch the gameplay demo](https://img.youtube.com/vi/QImtTx5jKb4/maxresdefault.jpg)](https://www.youtube.com/watch?v=QImtTx5jKb4)

## ✨ Features

- **Autonomous Ghost:** Wanders between randomly generated NavMesh destinations, with natural pauses and idle/walking animations.
- **Castle Guard AI:** Patrols a predefined route and reacts to the ghost using a finite state machine.
- **Field of View:** Detects the ghost through a directional vision cone and close-range awareness.
- **Alert & Escape:** Plays a fear reaction before fleeing toward a selected safe location.
- **Dynamic Navigation:** Uses Unity NavMesh for pathfinding and obstacle avoidance.
- **Animated Characters:** Smooth transitions between idle, wandering, patrolling, alert, and fleeing animations.

## 🧠 AI Architecture

The simulation uses two different approaches:

**Ghost — Script Graph**
- Random destination generation
- NavMesh destination validation
- Arrival detection and randomized waiting times

**Guard — State Graph**
- `Patrolling` → Follows a waypoint route
- `Alert` → Stops and reacts to the ghost
- `Flee` → Selects a safe location and escapes

Both agents are controlled using **Unity Visual Scripting**, without custom C# behaviour scripts.

## 🛠️ Tech Stack

- Unity 6 · Universal Render Pipeline (URP)
- Unity Visual Scripting
- Unity AI Navigation / NavMesh
- Animator Controllers
- Imported 3D models and animations

## Asset Ownership & Usage

All original 3D models, textures, and character animations showcased in this project are proprietary assets created by the author.

The Unity project and its original art assets are not publicly distributed. This repository serves as a technical showcase and portfolio demonstration of the game's AI systems.

**All rights reserved.** No permission is granted to reproduce, redistribute, or commercially use the original assets without prior authorization.

## 📌 Project Context

Developed as an academic project focused on game artificial intelligence, with an emphasis on autonomous movement, finite state machines, and agent interactions.

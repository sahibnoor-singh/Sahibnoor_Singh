<div align="center">
  <img src="https://via.placeholder.com/800x300.png?text=Tower+RTS+Banner" width="100%" alt="Tower RTS"/>
  
  <h1>3D Tactical RTS</h1>
  <p><b>Immersive Real-Time Strategy with Complex Resource Management</b></p>
</div>

<br/>

## 📌 Overview

**3D Tactical RTS** (Tower RTS) is a 3D real-time strategy game where players build bases, manage resources, and command armies in real-time battles. 

---

## 🎥 Demo


<div align="center">
  <img src="https://via.placeholder.com/600x400.png?text=TowerRTS+Demo+GIF" width="80%" alt="Gameplay Demo"/>
</div>

---

## 📸 Screenshots

<p align="center">
  <img src="https://via.placeholder.com/400x250.png?text=Base+Building" width="45%" />
  &nbsp;&nbsp;
  <img src="https://via.placeholder.com/400x250.png?text=Combat" width="45%" />
</p>

---

## ✨ Features

- **Base Building:** Construct and upgrade defensive towers and resource generators.
- **Unit Command:** Select and command multiple units with advanced pathfinding.
- **Resource Management:** Balance economy to fuel your army.

---

## 🛠 Tech Stack

- **Game Engine:** Unity 3D
- **Language:** C#
- **Key Systems:** NavMesh, custom Object Selection logic.

---

## 🏗 Architecture

```mermaid
graph TD
    A[Player Input] --> B(Selection Manager)
    B --> C{Unit Selected?}
    C -- Yes --> D[Command Manager]
    D --> E[NavMesh Agent (Move/Attack)]
    C -- No --> F[Building Placement]
```

---

## 📂 Folder Structure

```text
Assets/
├── 📁 Scripts/
│   ├── 📁 Units/         # Combat, Movement, Selection
│   ├── 📁 Buildings/     # Placement, Upgrades, Economy
│   └── 📁 Managers/      # GameManager, InputManager
└── 📁 Models/            # 3D Assets for units and environment
```

---

## 📈 Challenges Faced

1. **Pathfinding Bottlenecks:** When commanding 100+ units, Unity's default NavMesh Agent calculations caused frame drops.
   - **Solution:** Implemented flocking behavior and leader-follower pathing to reduce the number of individual path calculations.

---

## 💡 What I Learned

- Mastery of Unity's NavMesh system and its limitations.
- Implementing RTS-style drag-to-select boxes using screen-to-world raycasting.

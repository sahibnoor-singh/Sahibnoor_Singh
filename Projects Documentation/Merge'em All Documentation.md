<div align="center">
  <img src="https://via.placeholder.com/800x300.png?text=Merge'em+All+Banner" width="100%" alt="Merge'em All"/>
  
  <h1>Merge'em All</h1>
  <p><b>Satisfying Puzzle Game Focused on Infinite Progression</b></p>
</div>

<br/>

## 📌 Overview

**Merge'em All** is a merge puzzle game where players combine identical items to create higher-tier objects. 

---

## 🎥 Demo


<div align="center">
  <img src="https://via.placeholder.com/600x400.png?text=MergeEmAll+Demo+GIF" width="80%" alt="Gameplay Demo"/>
</div>

---

## ✨ Features

- **Infinite Progression:** Combine items infinitely to unlock rare tiers.
- **Offline Earnings:** Idle mechanics allow players to earn currency while away.
- **Daily Quests:** Integrated quest system to boost D1 and D7 retention.

---

## 🛠 Tech Stack

- **Game Engine:** Unity
- **Language:** C#
- **Saving System:** Custom JSON serialization for save states.

---

## 🏗 Architecture

```mermaid
graph TD
    A[Merge Controller] --> B{Items Overlap?}
    B -- Yes --> C{Are Items Same Tier?}
    C -- Yes --> D[Destroy Old Items]
    D --> E[Instantiate Next Tier]
    E --> F[Update Save File]
```

---

## 📈 Challenges Faced

- **Save File Corruption:** Players closing the app mid-merge could corrupt the JSON save state.
  - **Solution:** Implemented a dual-save system (backup + main) and only wrote to disk during stable idle states.

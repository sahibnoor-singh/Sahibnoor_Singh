<div align="center">
  <img src="https://via.placeholder.com/800x300.png?text=Snapchat+Lenses+Banner" width="100%" alt="Snapchat Lenses"/>
  
  <h1>Snapchat Lenses</h1>
  <p><b>Interactive Augmented Reality Experiences via SnapAR</b></p>
</div>

<br/>

## 📌 Overview

A collection of interactive Augmented Reality (AR) lenses developed using Snap's Lens Studio. These lenses utilize facial tracking, 3D object rendering, and custom scripting to create highly engaging experiences for Snapchat users.

---

## 🎥 Demo


<div align="center">
  <img src="https://via.placeholder.com/600x400.png?text=Lens+Demo+GIF" width="80%" alt="AR Demo"/>
</div>

---

## ✨ Features

- **Face Tracking:** High-fidelity masks that map perfectly to facial geometry.
- **Interactive Logic:** Lenses that react to facial gestures (e.g., opening mouth triggers an event).
- **Custom 3D Assets:** Imported and optimized 3D models for mobile AR performance.

---

## 🛠 Tech Stack

- **Platform:** Lens Studio
- **Scripting:** JavaScript
- **3D Pipeline:** Blender (for model preparation)

---

## 📈 Challenges Faced

- **Asset Size Limitations:** SnapAR imposes strict limits on lens bundle sizes (under 4MB ideally for fast loading).
  - **Solution:** Mastered texture compression, mesh decimation in Blender, and reusing materials to drastically reduce the footprint of the AR experiences.

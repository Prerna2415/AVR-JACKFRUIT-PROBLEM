🚀 Getting Started
1. Prerequisites
Node.js
(LTS recommended)

3. Install dependencies
If this is an NPM/Vite/Webpack project:
npm install
If it’s a simple static project with just Three.js in node_modules, this still makes sure dependencies are available.

3. Run the project
Using a dev server (example with Vite):
npm run dev

Then open:
http://localhost:5173    # Vite default

🎮 Controls
Adjust this list if your exact controls differ.
Camera (OrbitControls)
Rotate: Left Mouse Drag
Pan: Middle Mouse Drag or Shift + Left Mouse Drag
Zoom: Scroll Wheel

Cutting
Enter Cut Mode:
e.g. Press C key or click a “Cut Mode” UI button

Define Cut:
Click on the mesh to set the start point
Drag and release to define direction/extent of the cut

Confirm Cut:
On mouse release (pointerup), the app:
Computes the cutting plane

# Mesh Cutting System (Three.js)

A real-time **mesh cutting tool** built with [Three.js](https://threejs.org/).  
This project lets you interactively **slice 3D meshes** using a virtual cutting plane (knife) and visualizes the result in the browser.

---

## ✨ Features

- ✂️ **Interactive mesh cutting**
  - Click-and-drag to define a cutting plane
  - Mesh is split into two parts along the cut
- 🧱 **Supports arbitrary triangle meshes**
  - Works with most closed/manifold meshes
  - Supports custom imported models (with some limitations)
- 🧭 **Intuitive camera controls**
  - Orbit, pan, and zoom using mouse
- 🧪 **Debug visualization**
  - Optional display of cutting plane, normals, and intersection edges
- 🧱 **Modular architecture**
  - Core cutting logic is isolated from rendering & input
  - Easy to plug into other Three.js scenes

---
Passes it to MeshCutter
Replaces the original mesh with the newly cut parts

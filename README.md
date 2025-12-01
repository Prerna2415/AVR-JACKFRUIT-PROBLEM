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
Passes it to MeshCutter
Replaces the original mesh with the newly cut parts

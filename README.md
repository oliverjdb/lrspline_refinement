# LR B-Spline Refinement Explorer

Single-file React playgrounds for studying locally refined B-splines and their admissible refinement steps. Includes both 2D and 3D versions.

## Features

### 2D Version (`index.html`)
- Configurable polynomial degrees and starting tensor grid
- Guided point-pair workflow for inserting horizontal or vertical meshlines that obey LR rules
- Canvas overlays for Greville points, element coverage counts, and peeled-only views
- Peeling, knot-tuple peeling, and nesting-level analysis panels with interactive filtering
- Scrollable B-spline list for inspecting knot vectors and highlighting individual supports

### 3D Version (`index3d.html`)
- Extends LR B-spline refinement to 3D with meshfaces (planar regions) instead of meshlines
- Three.js visualization with interactive camera controls
- Click-to-select workflow for choosing refinement plane positions and extents
- Clickable Greville points to highlight individual B-spline supports
- Real-time element and meshface visualization

## Running the tool

1. Serve the folder from any static web server, e.g. `python3 -m http.server 8080`, or simply open `index.html` or `index3d.html` in any browser.
2. Open `http://localhost:8080` in your browser.
3. **2D**: Use "Show Reset Configuration" to pick degrees and element counts, then click point pairs to add refinements.
4. **3D**: Toggle "Refinement Mode" to select direction and click points to define rectangular meshface regions.

Everything lives in single HTML files, so no build step or dependency install is required.
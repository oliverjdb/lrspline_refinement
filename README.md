# LR B-Spline Refinement Explorer

A single-file React playground for studying locally refined B-splines and their admissible refinement steps.

## Features

- Configurable polynomial degrees and starting tensor grid
- Guided point-pair workflow for inserting horizontal or vertical meshlines that obey LR rules
- Canvas overlays for Greville points, element coverage counts, and peeled-only views
- Peeling, knot-tuple peeling, and nesting-level analysis panels with interactive filtering
- Scrollable B-spline list for inspecting knot vectors and highlighting individual supports

## Running the tool

1. Serve the folder from any static web server, e.g. `python3 -m http.server 8080`.
2. Open `http://localhost:8080` in your browser.
3. Use "Show Reset Configuration" to pick degrees and element counts, then apply.
4. Click a blue point to choose a start, then another valid point to complete the refinement segment.
5. Run the peeling/nesting actions for analytics and switch overlay modes to focus on Greville points or element counts.

Everything lives in `index.html`, so no build step or dependency install is required.
# Hand Frame

Hand-tracked AR in the browser. Hold an L shape with one hand and a 3D frame appears with an object inside. Use your other hand to dissolve it into particles and rebuild it as the next object.

## Run
1. Needs internet (loads three.js and MediaPipe from a CDN) and a webcam.
2. In this folder run: `python run.py` (opens http://localhost:8000). Or run `python -m http.server 8000` and open the link yourself.
3. Click Start camera and allow access. Use Chrome or Edge.

## Controls
- L shape (thumb + index out, other fingers curled): open the frame
- Other hand open palm: object dissolves and breaks into particles
- Other hand fist: particles rebuild as the next object
- Space: next object without a second hand. H: show or hide hand skeleton.

## Files
- index.html: the whole project (hand tracking, particle shapes, 3D frame)
- The Tree uses the texture maps in `models/tree/tree/` to build its 3D trunk and canopy.
- To add an object, write a generator like `lily` or `tree` and add it to the `SHAPES` list.

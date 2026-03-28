---
title: 3D Curve
parent: "Primitives"
nav_order: 13
---
# 3D Curve

Create and edit a 3D Bezier curve directly in the viewport. Unlike [Custom Path](../2d-paths/custom-path.md) which is flat, a 3D Curve has control points that can be positioned freely in all three dimensions, making it useful for defining spatial paths and freeform shapes.

<!-- IMAGE_NEEDED: A 3D S-curve in the viewport showing anchor points (squares) and handle control points (circles) with connection lines -->

## How to Use

1. Add a **3D Curve** from the Primitives panel
2. An S-shaped default curve appears with 3 control points
3. Drag **anchor points** (squares) to move curve endpoints
4. Drag **handle points** (circles) to adjust the curve shape between anchors
5. Rotate the camera to drag points in different directions — dragging always moves points parallel to the screen

## Controls

Each curve point has up to three interactive handles:

- **Anchor** (square) - The point the curve passes through. Dragging an anchor moves its handles with it.
- **Handle In** (circle) - Controls the curve shape arriving at this anchor
- **Handle Out** (circle) - Controls the curve shape leaving this anchor

Handles are connected to their anchor by thin lines for visual clarity.

## Handle Modes

Each anchor point has a handle mode that controls how its two handles relate:

- **Aligned** (default) - Handles stay co-linear through the anchor, producing smooth curves. Moving one handle automatically mirrors the other.
- **Free** - Handles move independently, allowing sharp direction changes at the anchor.
- **Auto** - Handles are automatically calculated from neighboring anchors for smooth interpolation.

## Tips

- To move a point in depth, rotate the camera 90 degrees and drag again
- The curve renders as a visible line in the viewport; it does not generate a solid mesh on its own
- Use 3D Curves for defining spatial paths and guide shapes

## Related

- [Custom Path](../2d-paths/custom-path.md) - Edit a 2D path with control points (flat, can be extruded)
- [Linear Extrude](../operations/path/linear-extrude.md) - Give a 2D path height

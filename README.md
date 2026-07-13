# 3D LEGO-Style Brick Designer

## Controls

- **Build mode:** click an upward-facing surface to place a brick; drag to orbit.
- **Select mode:** click a brick to select it.
- **Mouse wheel:** zoom.
- **Right drag:** pan.
- **R:** rotate the active brick by 90 degrees.
- **B / S:** switch to Build / Select mode.
- **Delete or Backspace:** delete the selected brick.
- **Ctrl/Cmd+Z:** undo.
- **Ctrl/Cmd+Shift+Z or Ctrl/Cmd+Y:** redo.

## Implemented safeguards

- Grid-aligned placement with corrected vertical centers.
- Occupancy-map collision detection and baseplate bounds.
- Optional one-stud support rule; side attachment is intentionally disabled.
- Click-versus-drag separation so orbiting does not place bricks.
- Versioned JSON save format with legacy-array migration and validation.
- Maximum import size, brick count, dimensions, and layer limits.
- Transactional imports: the current model is kept if parsing or validation fails.
- Cached brick geometry and materials, merged stud geometry, spatially clustered `InstancedMesh` rendering, and GPU cleanup.
- Keyboard-accessible controls, real color buttons, focus indicators, and responsive panels.

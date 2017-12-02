# Butterfly Tessellation

### Create plane
1. Remove extra units
1. Set units to mm
1. Switch to top view
1. Create a "plane"
    a. {Transform Panel -> Create Tab -> Plane}
1. Switch to Edit mode [tab]
1. Make sure you are in "Vertex Select Mode"
    1. {3D Scene (Edit Mode) -> "Vertex select"
1. Select all [a]
1. Subdivide the plane twice to get more points
    1. {Transform Panel (Edit Mode) -> Tools -> Subdivide}
1. Unselect Everything
1. Switch back to (Object Mode)
1. Switch to wireframe {3d scene -> display/shade -> wireframe}


## Cut and Rotate

### Cut

1. Create a Boolean Curve
    1. {Transform Panel -> Create Tab -> Boolean}
    1. Increase its size
        1. [s] for "scale" and move mouse up until it is big enough to
           see easily. {LMB} to accept.
    1. Rotate it to something close to the angle you want.
        1. [r] for "rotate" and move the mouse until it is where you
           want. You can be more specific, typing the axis and degrees,
           but that isnt necessary now.
        1. You can change the "pivot point" in the {3d scene -> pivot
           point} next to the wireframe mode dropdown.
    1. Switch to (edit mode)
    1. Enable "vertex snap" {3d scene -> type of element to snap ->
       vertex}
    1. Select a point (called "control point", not to be confused with
       the arms, which are called "handles"){RMB}
    1. grab [g] to move it near the desired point, then hold [Control]
       and move your mouse over a desired vertex to "snap" and it will
       align there perfectly.
    1. Grab and move the handles to modify the curve.
1. Switch to (object mode)
1. unselect all [a]
1. select the curve first, then hold down [Shift] and also select the
   plane with {RMB}.
1. Switch to (edit mode)
1. Cut the plane along the curve {Transform panel (edit mode) -> Knife
   project
1. Separate [p] the selection from the main plane.

### Rotate

1. Switch pivot point to 3d cursor {3d scene -> pivot center}
1. Select the piece to rotate.
1. Switch to (edit mode)
1. Make sure "vertex select" is active {3d scene-> vertex select}
1. {RMB} to select the vertex you want to rotate around.
1. [shift + s] -> cursor to selected to move the "3d cursor" (aka the
   target-looking thing)
1. DONT LEFT CLICK! If you do, it will move the 3d cursor, and youll
   have to move it back to the rotate point.
1. Switch back to object mode
1. [r] "rotate" along the [z] axis [180] degrees.
1. Cleanup: hide the bezier curve. {outliner scene -> bezier curve ->
   click the eye} You can also delete it.

### Recombine

1. Select both objects together in (object mode)
1. [Ctrl + j] "joins" them into 1 object


## Translational symmetry

1. Select 2 columns of vertices in the middle and dissolve them [x] -
   "Dissolve vertices"
1. Select the remaining middle column and [g] move it down the [y] axis
   [15] mm.
1. Round out the head.
    1. Using the same technique as the wing, draw a curve to cut a
       rounder section out of the tail.
    1. Create a new piece from the cut section, and [g] move to the top,
       using [Ctrl] to snap to vertex.
    1. join it with [Ctrl + j]
    1. Delete the extra edge on the bottom.
1. (Edit mode) Select all [a]. Remove the extra duplicated vertices
   {transform panel -> remove doubles}

## Reflectional Symmetry
1. [Shift + d] to "duplicate" Dont move the mouse! [Enter] to confirm.
   Make sure it is exactly in the same spot!
1. In (edit mode), select a vertex you want to rotate around and move
   the 3d cursor there [Shift + s] {cursor to selection}
1. Rotate [r] around the [y] axis [180] degrees.
1. Join the halves [Ctrl + j]
1. Remove doubles {transform panel -> remove doubles}

### Extrude into 3 dimensions
1. Click and drag {MMB} to rotate the view
1. Select the object
1. In (edit mode) make sure the whole shape is selected.
1. {transform panel -> extrude region} along the [z] axis [7] mm
    If this doesn't seem to work right, you may be extruding along a
    local z axis. While it is extruding, tap [z] until you rotate to
    "global" z, which will be straight up.


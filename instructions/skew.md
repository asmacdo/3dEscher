# Skewed tessellation
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
1. Mouse Move a column of points (in a line parallel to y axis)
    1. Select points in the middle using "Box select" [b]
    1. (dont click) "Grab" [g] the vertices to move them with your mouse.
    1. (dont click) Restrict movement to the y axis by pressing [y]
1. Precisely move another column of points
    1. Select points in the middle using "Box select" [b]
    1. "Precision Move":
      1. [g] to grab (no mouse)
      1. [y] to indicate axis to move (relative to current)
      1. Type [-20]. Since we are in mm units, this will move the
         selected vertices 20mm negatively along the y-axis. In Top
         View, this will appear to be "down".
1. Move a Row of points (they aren't quite parallel to x-axis anymore)
   Box select might still work, but lets select the points another way.
   [Shift]+{RMB} would work, but it is slow.
    1. Select the leftmost point with {RMB}
    1. Holding [Shift], Select the rightmost pioint with {RMB}. Only 2 points
       should be selected.
    1. {3D scene (Edit Mode) -> Select Menu -> Select Shortest Path}
    1. Move them with [g], either with the Mouse or with Precision.


1. Delete some points:
    1. {RMB} (still in Edit Mode) to select a point near the middle
    1. open the delete menu with [x|delete]
    1. Click "Disolve Vertices" to remove the point without creating a
       hole.
    1. {RMB} to select a different point in the middle.
    1. Delete [x]
    1. Click "Vertices" to delete the vertex, which will create a hole.
    1. Switch to Object Mode [tab] to see it.
1. Connect some points: Select 2 points that you'd like to connect with
   a line (called an "Edge" in Blender). [f]
1. Select all the points around the hole you made.
1. press [f] to connect them with edges and faces.


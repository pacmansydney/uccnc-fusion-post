# Modified Fusion UCCNC Post Libraries

## uccnc-circular.cps

- Circular planes are enabled in all planes, not just PLANE_XY by default (allowedCircularPlanes = undefined).
- Output G17/G18/G19 commands as appropriate. By default, gPlaneModal is disabled in onOpen() resulting in these GCodes not being output.
- Reset the plane by issuing the G17 command in various places such as onOpen, onSelection and onSelectionEnd just like the Masso Post.

## uccnc-circular-clearance.cps

- In addition to the changes above, changes the default Safe Retracts to Clearance Height instead of G53.

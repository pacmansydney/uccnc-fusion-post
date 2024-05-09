# Modified Fusion UCCNC Post Libraries

USE AT YOUR OWN RISK! THIS LIBRARY HAS BEEN PUBLISHED FOR TESTING PURPOSES WITH THE INTENTION OF PUSHING THESE CHANGES UPSTREAM ONCE TESTED

## uccnc.cps

- This is the unmodified UCCNC Post Library published by Autodesk, provided for comparison purposes.

## uccnc-circular.cps

- Circular moves (G2/G3) are enabled in all planes not just the default PLANE_XY (allowedCircularPlanes = undefined).
- Output G17/G18/G19 commands as appropriate. By default, gPlaneModal is disabled in onOpen() resulting in these GCodes not being output.
- Reset the plane by issuing the G17 command in various places such as onOpen, onSelection and onSelectionEnd like the Masso Post Library and others do.

## uccnc-circular-clearance.cps

- In addition to the changes above, changes the default Safe Retracts to Clearance Height instead of G53.

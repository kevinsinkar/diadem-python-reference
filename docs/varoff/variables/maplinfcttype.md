---
title: "MapLinFctType"
description: "Specifies the type of function that is to be mapped."
---

# MapLinFctType

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: MapLinFctType

Specifies the type of function that is to be mapped.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For digital functions such as spikes and stairs the maximum step width of the new x-range must be smaller than half of the minimum step width of the original x-range. This way you can avoid level changes. DIAdem also can assign two values Y(Xa), Y(Xb) to the same interpolation value X1. In this case DIAdem takes the value (y(xa) or y(xb)) of which the interpolation point (xa or xb) is closest to the new interpolation value x1. If both of the original interpolation points (xa and xb) are the same distance from the new interpolation value (x1), the y-value of the lower interpolation point is the result.</td></tr></table>
</div>

---

*Source: `VarOff/MapLinFctType.htm`*

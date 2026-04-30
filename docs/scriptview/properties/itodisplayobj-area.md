---
title: "IToDisplayObj.Area"
description: "Returns the area in DIAdem VIEW that contains the executing object."
---

# IToDisplayObj.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for DisplayObj

Returns the area in DIAdem VIEW that contains the executing object.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyArea = oMyObj.Area
dd.MsgBoxDisp(oMyArea.DisplayObjType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_IToDisplayObj.htm`*

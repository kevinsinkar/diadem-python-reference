---
title: "IToPictureInt.Area"
description: "Returns the area in DIAdem VIEW that contains a graphic."
---

# IToPictureInt.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for Picture

Returns the area in DIAdem VIEW that contains a graphic.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "Picture"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyObj.FileName = "Example.png"
dd.MsgBoxDisp("Name " + oMyObj.Area.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_IToPictureInt.htm`*

---
title: "IToVideoInt.Area"
description: "Returns the area in DIAdem VIEW that contains a video."
---

# IToVideoInt.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for Video

Returns the area in DIAdem VIEW that contains a video.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "Video"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyObj.FileName = "Example.wmv"
dd.MsgBoxDisp("Name " + oMyObj.Area.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_IToVideoInt.htm`*

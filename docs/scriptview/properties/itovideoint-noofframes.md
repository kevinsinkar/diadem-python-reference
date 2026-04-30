---
title: "IToVideoInt.NoOfFrames"
description: "Returns the number of pictures in a video file in DIAdem VIEW."
---

# IToVideoInt.NoOfFrames

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: NoOfFrames for Video

Returns the number of pictures in a video file in DIAdem VIEW.

## Signature

```python
obj.NoOfFrames
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "Video"
oMyObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyObj.FrameRate = int(oMyObj.NoOfFrames/60)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_NoOfFrames_IToVideoInt.htm`*

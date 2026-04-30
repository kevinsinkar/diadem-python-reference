---
title: "IToVideoInt.KeepRatio"
description: "Specifies whether DIAdem maintains the height/width ratio of videos in DIAdem VIEW."
---

# IToVideoInt.KeepRatio

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: KeepRatio for Video

Specifies whether DIAdem maintains the height/width ratio of videos in DIAdem VIEW.

## Signature

```python
obj.KeepRatio
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "Video"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.FileName = "C:\\Videos\\SideCrash.wmv"
oMyObj.KeepRatio = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Displaying Videos and Data Synchronously</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_KeepRatio_IToVideoInt.htm`*

---
title: "IToPictureInt.KeepRatio"
description: "Specifies whether DIAdem maintains the height/width ratio of graphics in DIAdem VIEW."
---

# IToPictureInt.KeepRatio

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: KeepRatio for Picture

Specifies whether DIAdem maintains the height/width ratio of graphics in DIAdem VIEW.

## Signature

```python
obj.KeepRatio
```

## Python example

```python
dd.View.ActiveSheet.ActiveArea.DisplayObjType = "Picture"
oMyObj = dd.View.ActiveSheet.ActiveArea.DisplayObj
oMyObj.FileName = "C:\\Pictures\\Example.png"
oMyObj.KeepRatio = True
```

---

*Source: `Scriptview/properties/VIEW_property_KeepRatio_IToPictureInt.htm`*

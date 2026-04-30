---
title: "IToBirdsEyeViewObjectInt.LabelColorAuto"
description: "Specifies whether the color of the label of a dynamic object in a bird's eye view display in DIAdem VIEW corresponds to the color of the dynamic objects."
---

# IToBirdsEyeViewObjectInt.LabelColorAuto

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: LabelColorAuto for BirdsEyeViewDynamicObject

Specifies whether the color of the label of a dynamic object in a bird's eye view display in DIAdem VIEW corresponds to the color of the dynamic objects.

## Signature

```python
obj.LabelColorAuto
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddDynamicObject("[1]/[1]","[1]/[2]","[1]/[3]")
oMyObject.LabelChannelName = "[1]/[4]"
oMyObject.LabelColorAuto = False
oMyObject.LabelColor = "blue"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_LabelColorAuto_IToBirdsEyeViewObjectInt.htm`*

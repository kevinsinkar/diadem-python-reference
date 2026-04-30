---
title: "IToBirdsEyeViewObjectInt.LabelColorRGB"
description: "Specifies whether the color of the label of a dynamic object in a bird's eye view display in DIAdem VIEW corresponds to the color of a dynamic object. DIAdem on"
---

# IToBirdsEyeViewObjectInt.LabelColorRGB

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: LabelColorRGB for BirdsEyeViewDynamicObject

Specifies whether the color of the label of a dynamic object in a bird's eye view display in DIAdem VIEW corresponds to the color of a dynamic object. DIAdem only includes the color if the LabelColor property has the value other colors and the LabelColorAuto property has the value FALSE .

## Signature

```python
obj.LabelColorRGB
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddDynamicObject("[1]/[1]","[1]/[2]","[1]/[3]")
oMyObject.LabelChannelName = "[1]/[4]"
oMyObject.LabelColorAuto = False
oMyObject.LabelColor = "other colors"
oMyObject.LabelColorRGB = dd.RGB(0,0,221)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_LabelColorRGB_IToBirdsEyeViewObjectInt.htm`*

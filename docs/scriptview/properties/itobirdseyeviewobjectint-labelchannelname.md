---
title: "IToBirdsEyeViewObjectInt.LabelChannelName"
description: "Specifies the name of the channel that contains the labels of a dynamic object in a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewObjectInt.LabelChannelName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: LabelChannelName for BirdsEyeViewDynamicObject

Specifies the name of the channel that contains the labels of a dynamic object in a bird's eye view display in DIAdem VIEW.

## Signature

```python
obj.LabelChannelName
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

*Source: `Scriptview/properties/VIEW_property_LabelChannelName_IToBirdsEyeViewObjectInt.htm`*

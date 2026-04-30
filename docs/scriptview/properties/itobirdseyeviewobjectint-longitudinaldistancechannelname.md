---
title: "IToBirdsEyeViewObjectInt.LongitudinalDistanceChannelName"
description: "Specifies the name of the channel that contains the distance in longitudinal direction of a dynamic object in a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewObjectInt.LongitudinalDistanceChannelName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: LabelColorRGB for BirdsEyeViewDynamicObject

Specifies the name of the channel that contains the distance in longitudinal direction of a dynamic object in a bird's eye view display in DIAdem VIEW.

## Signature

```python
obj.LongitudinalDistanceChannelName
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddDynamicObject("[1]/[1]","[1]/[2]","[1]/[3]")
dd.MsgBoxDisp("Synchronisation channel: " + oMyObject.SynchronisationChannelName + "\r\n" + "Lateral distance: " + oMyObject.LateralDistanceChannelName + "\r\n" + "Longitudinal distance: " + oMyObject.LongitudinalDistanceChannelName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_LongitudinalDistanceChannelName_IToBirdsEyeViewObjectInt.htm`*

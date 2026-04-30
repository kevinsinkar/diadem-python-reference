---
title: "IToBirdsEyeViewObjectInt.LateralDistanceChannelName"
description: "Specifies the name of the channel that contains the lateral distance of a dynamic object in a bird's eye view display in DIAdem VIEW."
---

# IToBirdsEyeViewObjectInt.LateralDistanceChannelName

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: LateralDistanceChannelName for BirdsEyeViewDynamicObject

Specifies the name of the channel that contains the lateral distance of a dynamic object in a bird's eye view display in DIAdem VIEW.

## Signature

```python
obj.LateralDistanceChannelName
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

*Source: `Scriptview/properties/VIEW_property_LateralDistanceChannelName_IToBirdsEyeViewObjectInt.htm`*

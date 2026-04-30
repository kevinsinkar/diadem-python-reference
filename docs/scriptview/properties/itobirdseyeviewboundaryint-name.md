---
title: "IToBirdsEyeViewBoundaryInt.Name"
description: "Specifies the name of a dynamic object in a bird's eye view display in DIAdem VIEW. As the dynamic object is identified by its name, the name must be unique and"
---

# IToBirdsEyeViewBoundaryInt.Name

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Name for BirdsEyeViewBoundary

Specifies the name of a dynamic object in a bird's eye view display in DIAdem VIEW. As the dynamic object is identified by its name, the name must be unique and may not be allocated more than once.

## Signature

```python
obj.Name
```

## Python example

```python
oMySheet = dd.View.Sheets.Add("NewBirdsEyeView")
oMySheet.ActiveArea.DisplayObjType = "BirdsEyeView"
oMyObjects = dd.View.ActiveSheet.ActiveArea.DisplayObj.BirdsEyeViewObjects
oMyObject = oMyObjects.AddDynamicObject("[1]/[1]","[1]/[2]","[1]/[3]")
dd.LogfileWrite("Dynamic object: " + oMyObject.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>
	 </h2>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Name_IToBirdsEyeViewBoundaryInt.htm`*

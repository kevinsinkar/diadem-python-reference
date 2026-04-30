---
title: "ToActionObjButtonInt.Tooltip"
description: "Specifies the tooltip for a bar element. If you idle the mouse on a bar element, the tooltip appears."
---

# ToActionObjButtonInt.Tooltip

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Tooltip for ActionObjButton

Specifies the tooltip for a bar element. If you idle the mouse on a bar element, the tooltip appears.

## Signature

```python
obj.Tooltip
```

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyButton")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton", "CustomButton")
    oMyActionObj.Picture = "favicon.ico"
    oMyActionObj.Tooltip = "MyButton"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Tooltip_ToActionObjButtonInt.htm`*

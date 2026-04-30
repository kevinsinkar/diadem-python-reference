---
title: "ToActionObjCheckInt.Check"
description: "Specifies whether the button that displays a status is enabled in the DIAdem interface."
---

# ToActionObjCheckInt.Check

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Check for ActionObjCheckbutton

Specifies whether the button that displays a status is enabled in the DIAdem interface.

## Signature

```python
obj.Check
```

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyObjCheck1")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyObjCheck1", "CustomCheckButton")
    oMyActionObj.Tooltip = "MyObjCheck1"
    oMyActionObj.Check   = True
dd.BarManager.Bars("MyBar").UsedActionObjs.Add(oMyActionObj)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Check_ToActionObjCheckInt.htm`*

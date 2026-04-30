---
title: "ToActionObjCheckInt.Tooltip"
description: "Specifies the tooltip for a bar element. If you idle the mouse on a bar element, the tooltip appears."
---

# ToActionObjCheckInt.Tooltip

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Tooltip for ActionObjCheckbutton

Specifies the tooltip for a bar element. If you idle the mouse on a bar element, the tooltip appears.

## Signature

```python
obj.Tooltip
```

## Python example

```python
oFloating = dd.BarManager.ActionObjs.Add("PtlFloatingOnOff", "CustomCheckButton")
oFloating.Tooltip = "Floating Portal"
oFloating.Picture  = "Portal.ico"
oFloating.OnRefreshCode.Code = "this.Check = PtlFloating"
oFloating.OnClickCode.Code = "PtlFloating = not this.Check"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oFloating)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Tooltip_ToActionObjCheckInt.htm`*

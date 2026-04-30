---
title: "ToBarManagerUIInt.DesktopModified"
description: "Specifies whether the bar definition has changed since DIAdem launched or since a desktop file was loaded or saved. DIAdem indicates that the bar definition is "
---

# ToBarManagerUIInt.DesktopModified

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: DesktopModified for BarManager

Specifies whether the bar definition has changed since DIAdem launched or since a desktop file was loaded or saved. DIAdem indicates that the bar definition is changed if you changed the DIAdem interface with a script or if you changed the default settings via the setting Predefine Setting in the context menu. If the DesktopModified property contains the property TRUE , a prompt asks when DIAdem closes whether DIAdem should save the changed bar definition. Assign the value FALSE to the DesktopModified property so that DIAdem does not display a confirmation prompt after the bar definition is changed. If you make changes to the bar definition after you have assigned BarManager.DesktopModified = FALSE , the DesktopModified property contains the value TRUE again.

## Signature

```python
obj.DesktopModified
```

## Python example

```python
if not (dd.BarManager.ActionObjs.Exists("MyObjCheck1")) :
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyObjCheck1", "CustomCheckButton")
    oMyActionObj.Tooltip = "MyObjCheck1"
    oMyActionObj.Check   = True
dd.BarManager.Bars("MyBar").UsedActionObjs.Add(oMyActionObj)
dd.BarManager.DesktopModified = False
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../methods/tobarmanagerint-ismodified/">IsModified</a> | <a href="#" data-unresolved="1">Objects Ov erview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_DesktopModified_ToBarManagerUIInt.htm`*

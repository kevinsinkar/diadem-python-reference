---
title: "ToBarManagerUIInt.Create"
description: "Creates a further bar manager that reads in a bar definition or that generates an empty bar definition. DIAdem does not use this bar manager for display on the "
---

# ToBarManagerUIInt.Create

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Create for BarManager

Creates a further bar manager that reads in a bar definition or that generates an empty bar definition. DIAdem does not use this bar manager for display on the interface. If you do not specify a bar definition name, DIAdem generates an empty bar definition that only contains the panels collection and three empty bars per panel. Use the empty bar definition to generate a bar definition that only contains user-defined bars which you can provide to other users.

## Signature

```python
return_value = obj.Create(FileName)
```

## Python example

```python
oMyBardef = dd.BarManager.Create("")
oMyActionObj = oMyBarDef.ActionObjs.Add("MyObjPopup", "CustomPopUp")
oMyActionObj.Tooltip = "Opens ANAMain"
oMyActionObj.BarID   = "ANAMain"
oMyBarDef.Bars("SCRGroup").UsedActionObjs.Add(oMyActionObj)
oMyBarDef.Save("MyBarDef.bdn")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../tobarmanagerint-import/">Import</a> | <a href="../tobarmanagerint-saveasdeployment/">SaveAsDeployment</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Create_ToBarManagerUIInt.htm`*

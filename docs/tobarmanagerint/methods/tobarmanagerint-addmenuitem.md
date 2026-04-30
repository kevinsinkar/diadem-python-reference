---
title: "ToBarManagerInt.AddMenuItem"
description: "Adds a menu item to a bar. The method returns the ActionObjButton object, which contains the new menu item. The new bars belong to an additional bar manager not"
---

# ToBarManagerInt.AddMenuItem

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: AddMenuItem for BarManagerUnattached

Adds a menu item to a bar. The method returns the ActionObjButton object, which contains the new menu item. The new bars belong to an additional bar manager not used for the bar display in DIAdem. The methods AddMenuBar and AddMenuItem are used to create individual menu items. The new bar is usually a menu bar but can also appear as a symbol bar. DIAdem automatically allocates the IDs for the created objects. If you want to use the bars several times, use the other objects and methods of the BarManager object.

## Signature

```python
return_value = obj.AddMenuItem(TargetBarObjOrID, Caption, Function, Position)
```

## Python example

```python
oMyBardef = dd.BarManager.Create("")
oMyMenuBar = oMyBarDef.AddMenuBar("REPMenuMain", "My Bar", 0)
oMyBarDef.AddMenuItem(oMyMenuBar, "Show Message Box", "print(\"Hello World\")", 0)
oMyBarDef.AddMenuItem(oMyMenuBar, "Show Time", "print(CurrTime)", 0)
oMyMenuBar.UsedActionObjs.Add("Separator")
oMyBarDef.AddMenuItem(oMyMenuBar, "Reset Bars", "Call BarManager.Reset", 0)
oMyBarDef.Save("MyBarDef.bdn")
#Call BarManager.Import("MyBarDef.bdn",eImportAsk)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_AddMenuItem_ToBarManagerInt.htm`*

---
title: "ToBarManagerUIInt.AddMenuBar"
description: "Adds a menu bar to a bar. The method creates an ActionObjPopup object in the target bar containing the new menu bar. The method returns the Bar object which con"
---

# ToBarManagerUIInt.AddMenuBar

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: AddMenuBar for BarManager

Adds a menu bar to a bar. The method creates an ActionObjPopup object in the target bar containing the new menu bar. The method returns the Bar object which contains the new menu item. Use the AddMenuItem method to fill the new menu bar with menu items. The methods AddMenuBar and AddMenuItem are used to create individual menu items. The new bar is usually a menu bar but can also appear as a symbol bar. DIAdem automatically allocates the IDs for the created objects. If you want to use the bars several times, use the other objects and methods of the BarManager object.

## Signature

```python
return_value = obj.AddMenuBar(TargetBarObjOrID, Caption, Position)
```

## Python example

```python
oMyMenuBar = dd.BarManager.AddMenuBar("REPMenuMain", "My Bar", 0)
dd.BarManager.AddMenuItem(oMyMenuBar, "Show Message Box", "print(\"Hello World\")", 0)
dd.BarManager.AddMenuItem(oMyMenuBar, "Show Time", "print(CurrTime)", 0)
oMyMenuBar.UsedActionObjs.Add("Separator")
dd.BarManager.AddMenuItem(oMyMenuBar, "Reset Bars", "Call BarManager.Reset", 0)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_AddMenuBar_ToBarManagerUIInt.htm`*

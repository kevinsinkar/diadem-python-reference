---
title: "ToBarManagerUIInt.AddMenuItem"
description: "Adds a menu item to a bar. The method returns the ActionObjButton object which contains the new menu item. The methods AddMenuBar and AddMenuItem are used to cr"
---

# ToBarManagerUIInt.AddMenuItem

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: AddMenuItem for BarManager

Adds a menu item to a bar. The method returns the ActionObjButton object which contains the new menu item. The methods AddMenuBar and AddMenuItem are used to create individual menu items. The new bar is usually a menu bar but can also appear as a symbol bar. DIAdem automatically allocates the IDs for the created objects. If you want to use the bars several times, use the other objects and methods of the BarManager object.

## Signature

```python
return_value = obj.AddMenuItem(TargetBarObjOrID, Caption, Function, Position)
```

## Python example

```python
oNewButton = dd.BarManager.AddMenuItem("REPMenuFile", "Layout with 2D Axissystem", "Call Report.NewLayout", 2)()
oNewButton.OnClickCode.AddCodeLine("Call Report.ActiveSheet.Objects.Add(eReportObject2DAxisSystem, \"\")")
oNewButton.OnClickCode.AddCodeLine("Call Report.Refresh")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_AddMenuItem_ToBarManagerUIInt.htm`*

---
title: "ToBarListInt.Exists"
description: "Checks whether a bar with a specific name exists."
---

# ToBarListInt.Exists

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Exists for Bars

Checks whether a bar with a specific name exists.

## Signature

```python
bExists = Object.Exists(ID)
```

## Python example

```python
sgBarId = "MyBar"
if (not dd.BarManager.Bars.Exists(sgBarId)) :
    dd.BarManager.Bars.Add(sgBarId)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Exists_ToBarListInt.htm`*

---
title: "ToBarManagerUIInt.IsModified"
description: "Specifies whether the bar definition has changed compared to the saved bar definition file."
---

# ToBarManagerUIInt.IsModified

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: IsModified for BarManager

Specifies whether the bar definition has changed compared to the saved bar definition file.

## Signature

```python
bIsModified = Object.IsModified
```

## Python example

```python
if dd.BarManager.IsModified :
    dd.BarManager.Save("MyDefinition.bdn")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_IsModified_ToBarManagerUIInt.htm`*

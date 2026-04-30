---
title: "ToUsedBarListInt.Count"
description: "Returns the number of references to bars in a DIAdem panel or in the DIAdem main window."
---

# ToUsedBarListInt.Count

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Count for UsedBars

Returns the number of references to bars in a DIAdem panel or in the DIAdem main window.

## Signature

```python
obj.Count
```

## Python example

```python
dd.MsgBoxDisp("Number of bars: " + dd.Barmanager.Shell.UsedBars.Count)
```

```python
for oMyPanel in dd.BarManager.Panels:
    dd.MsgBoxDisp(oMyPanel.ID + ", " + oMyPanel.UsedBars.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Count_ToUsedBarListInt.htm`*

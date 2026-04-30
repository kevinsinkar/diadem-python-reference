---
title: "ToActionObjPopupInt.Reset"
description: "Restores the base properties of the base type for buttons that open a bar. The base properties of the buttons comprise the graphic to be displayed, the tooltip,"
---

# ToActionObjPopupInt.Reset

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Reset for ActionObjPopup

Restores the base properties of the base type for buttons that open a bar. The base properties of the buttons comprise the graphic to be displayed, the tooltip, and the graphic to be opened.

## Signature

```python
obj.Reset
```

## Python example

```python
#Sets BarID, Tooltip and Picture
dd.BarManager.ActionObjs("ANACrashAnalysis").BarID = "ANAMain"
dd.BarManager.ActionObjs("ANACrashAnalysis").Tooltip = "Crash Functions"
dd.BarManager.ActionObjs("ANACrashAnalysis").Picture = "MyCrash.ico"

#Resets BarID, Tooltip and Picture
dd.BarManager.ActionObjs("ANACrashAnalysis").Reset()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Reset_ToActionObjPopupInt.htm`*

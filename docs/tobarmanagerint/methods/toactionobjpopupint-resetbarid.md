---
title: "ToActionObjPopupInt.ResetBarID"
description: "Replaces the name of the bar that opens when the bar element is clicked with the bar name that is entered in the base type of the bar element."
---

# ToActionObjPopupInt.ResetBarID

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: ResetBarID for ActionObjPopup

Replaces the name of the bar that opens when the bar element is clicked with the bar name that is entered in the base type of the bar element.

## Signature

```python
obj.ResetBarID
```

## Python example

```python
#Sets BarID
dd.BarManager.ActionObjs("ANACrashAnalysis").BarID = "ANAMain"

#Resets BarID
dd.BarManager.ActionObjs("ANACrashAnalysis").ResetBarID
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_ResetBarID_ToActionObjPopupInt.htm`*

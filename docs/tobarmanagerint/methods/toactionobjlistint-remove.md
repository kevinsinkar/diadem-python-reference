---
title: "ToActionObjListInt.Remove"
description: "Deletes an element from the ActionObjs collection and also deletes all references to this element in the UsedActionObjs collections."
---

# ToActionObjListInt.Remove

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Remove for ActionObjs

Deletes an element from the ActionObjs collection and also deletes all references to this element in the UsedActionObjs collections.

## Signature

```python
obj.Remove(IDOrIndex)
```

## Python example

```python
if dd.BarManager.ActionObjs.Exists("MyPopup") :
    dd.BarManager.ActionObjs.Remove("MyPopup")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Remove_ToActionObjListInt.htm`*

---
title: "ToActionObjListInt.Copy"
description: "Duplicates an ActionObj object and adds the new object to the collection behind the object to be duplicated."
---

# ToActionObjListInt.Copy

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Copy for ActionObjs

Duplicates an ActionObj object and adds the new object to the collection behind the object to be duplicated.

## Signature

```python
return_value = obj.Copy(IDOrIndex, NewID)
```

## Python example

```python
dd.BarManager.ActionObjs.Copy("ANADlgChnAdd","MyANADlgChnAdd")
dd.BarManager.ActionObjs("MyANADlgChnAdd").Tooltip = "My channel add function"
dd.Barmanager.Bars("ANAMain").UsedActionObjs.Insert("MyANADlgChnAdd",5)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Copy_ToActionObjListInt.htm`*

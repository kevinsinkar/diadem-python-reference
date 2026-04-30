---
title: "ToActionObjListInt.Add"
description: "Adds an object to the ActionObjs collection and returns an ActionObj object."
---

# ToActionObjListInt.Add

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Add for ActionObjs

Adds an object to the ActionObjs collection and returns an ActionObj object.

## Signature

```python
return_value = obj.Add(ID, BaseID)
```

## Python example

```python
if dd.BarManager.ActionObjs.Exists("MyButton") :
    oMyActionObj = dd.BarManager.ActionObjs("MyButton")
else:
    oMyActionObj = dd.BarManager.ActionObjs.Add("MyButton","CustomButton")
    oMyActionObj.Tooltip = "MyButton"
    oMyActionObj.Picture = "favicon.ico"
dd.BarManager.Bars("SCRMain").UsedActionObjs.Add(oMyActionObj)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Add_ToActionObjListInt.htm`*

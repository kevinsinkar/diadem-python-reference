---
title: "ToActionObjListInt.GetUniqueID"
description: "Checks whether the name of a bar element is valid and unique. The name of a bar element can contain the characters a to z, A to Z, 0 to 9, the hyphen, and the u"
---

# ToActionObjListInt.GetUniqueID

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: GetUniqueID for ActionObjs

Checks whether the name of a bar element is valid and unique. The name of a bar element can contain the characters a to z, A to Z, 0 to 9, the hyphen, and the underscore. DIAdem replaces invalid characters with the underscore. If the specified name already exists, DIAdem generates a new name. To do so, DIAdem adds an underscore and a number to the existing name.

## Signature

```python
sGetUniqueID = Object.GetUniqueID(ID)
```

## Python example

```python
dd.MsgBoxDisp("Name of element: " + dd.BarManager.ActionObjs.GetUniqueID("MyButton"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_GetUniqueID_ToActionObjListInt.htm`*

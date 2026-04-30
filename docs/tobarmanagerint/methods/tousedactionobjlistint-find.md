---
title: "ToUsedActionObjListInt.Find"
description: "Searches the UsedActionObjs collection for a reference to a bar element. If you specify the start position of the search, you can also find multiple references."
---

# ToUsedActionObjListInt.Find

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Find for UsedActionObjs

Searches the UsedActionObjs collection for a reference to a bar element. If you specify the start position of the search, you can also find multiple references.

## Signature

```python
iFind = Object.Find(ActionObjOrID, StartPos)
```

## Python example

```python
Found = dd.BarManager.Bars("SCRMain").UsedActionObjs.Find("Separator",1)
while ((Found > 0)):
    dd.LogfileWrite("Separator at position " + Found )
    Start = Found + 1
    Found = dd.BarManager.Bars("SCRMain").UsedActionObjs.Find("Separator",Start)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Find_ToUsedActionObjListInt.htm`*

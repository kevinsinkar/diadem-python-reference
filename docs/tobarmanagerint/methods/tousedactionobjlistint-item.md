---
title: "ToUsedActionObjListInt.Item"
description: "Returns the Bar element associated with a specific index or with a specific name. Note If a bar contains several consecutive separating lines, DIAdem displays o"
---

# ToUsedActionObjListInt.Item

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Item for UsedActionObjs

Returns the Bar element associated with a specific index or with a specific name. Note If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If this is the case, the number of visible bar elements does not correspond with the number of bar elements contained in the Count property.

## Signature

```python
return_value = obj.Item(IDOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table3">
<tr>
<td class="Icon" width="415"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If this is the case, the number of visible bar elements does not correspond with the number of bar elements contained in the <a href="../../properties/tousedactionobjlistint-count/">Count</a> property.</td>
</tr>
</table>
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
FirstBar = dd.BarManager.Bars(1)
dd.MsgBoxDisp("Name of first element: " + FirstBar.UsedActionObjs.Item(1).ID)
dd.MsgBoxDisp("Name of first element: " + FirstBar.UsedActionObjs(1).ID)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Item_ToUsedActionObjListInt.htm`*

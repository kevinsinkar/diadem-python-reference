---
title: "ToUsedActionObjListInt.Insert"
description: "Adds a reference to a bar element to a specified position in the UsedActionObjs collection. If you specify a position that is larger than the number of elements"
---

# ToUsedActionObjListInt.Insert

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Insert for UsedActionObjs

Adds a reference to a bar element to a specified position in the UsedActionObjs collection. If you specify a position that is larger than the number of elements that already exist, DIAdem adds the reference to the bar element at the end. Note If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If this is the case, the number of visible bar elements does not correspond with the number of bar elements contained in the Count property.

## Signature

```python
obj.Insert(ActionObjOrID, Index)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon" width="415"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If this is the case, the number of visible bar elements does not correspond with the number of bar elements contained in the <a href="../../properties/tousedactionobjlistint-count/">Count</a> property.</td>
</tr>
</table>
</div>

## Python example

```python
oActionObj = dd.BarManager.ActionObjs.Add("MyButton", "CustomButton")
oActionObj.Tooltip = "MyButton"
oActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"Hello\")"
dd.Barmanager.Bars("SCRMain").UsedActionObjs.Insert("MyButton",9)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Insert_ToUsedActionObjListInt.htm`*

---
title: "ToUsedActionObjListInt.Remove"
description: "Removes a reference to the UsedActionObjs collection. Note If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If "
---

# ToUsedActionObjListInt.Remove

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Remove for UsedActionObjs

Removes a reference to the UsedActionObjs collection. Note If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If this is the case, the number of visible bar elements does not correspond with the number of bar elements contained in the Count property.

## Signature

```python
obj.Remove(IDOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2">
<tr>
<td class="Icon" width="415"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  If a bar contains several consecutive separating lines, DIAdem displays only one separating line. If this is the case, the number of visible bar elements does not correspond with the number of bar elements contained in the <a href="../../properties/tousedactionobjlistint-count/">Count</a> property.</td>
</tr>
</table>
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If a bar contains a reference multiple times, DIAdem removes the first reference it finds.</td>
</tr>
</table>
</div>

## Python example

```python
dd.BarManager.Bars("ANAMain").UsedActionObjs.Remove(1)
```

```python
dd.BarManager.Bars("DIAPanels").UsedActionObjs.Remove("DIAPanelSCRIPT")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Remove_ToUsedActionObjListInt.htm`*

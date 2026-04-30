---
title: "ToActionObjCheckInt.ID"
description: "Specifies the name of the bar element in the ActionObj collection. DIAdem does not distinguish between uppercase and lowercase for the specified name. The name "
---

# ToActionObjCheckInt.ID

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: ID for ActionObjCheckbutton

Specifies the name of the bar element in the ActionObj collection. DIAdem does not distinguish between uppercase and lowercase for the specified name. The name is unique in the ActionObj collection.

## Signature

```python
obj.ID
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If you change the name of a bar element, you also change all the references to the bar element in the <a href="../../collections/usedactionobjs/">UsedActionObjs</a> collections.</td>
</tr>
</table>
</div>

## Python example

```python
if dd.BarManager.ActionObjs.Exists("MyCheckButton") :
    dd.BarManager.ActionObjs("MyCheckButton").ID = "MyCheckButton_1"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_ID_ToActionObjCheckInt.htm`*

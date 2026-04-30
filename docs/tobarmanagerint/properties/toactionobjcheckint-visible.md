---
title: "ToActionObjCheckInt.Visible"
description: "Specifies whether the button that displays a status is visible. Note DIAdem does not save the Visible property in the bar definition. Note Use the Visible prope"
---

# ToActionObjCheckInt.Visible

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Visible for ActionObjCheckbutton

Specifies whether the button that displays a status is visible. Note DIAdem does not save the Visible property in the bar definition. Note Use the Visible property only within the OnRefreshCode event.

## Signature

```python
obj.Visible
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>DIAdem does not save the <span class="Monospace">Visible</span> property in the bar definition.</td>
</tr>
</table>
<table class="Borderless" id="table3">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Use the <span class="Monospace">Visible</span> property only within the <a href="../toactionobjcheckint-onrefreshcode/">OnRefreshCode</a> event.</td>
</tr>
</table>
</div>

## Python example

```python
oMyActionObj = dd.BarManager.ActionObjs.Add("MyCheckButton","CustomCheckButton")
oMyActionObj.Tooltip = "Floating portal"
oMyActionObj.Picture = "Portal.ico"
oMyActionObj.OnClickCode.Code = "PtlFloating = not This.Check"
oMyActionObj.OnRefreshCode.Code = "This.Check = PtlFloating" + "\r\n" + "This.Visible = (WndName=\"VIEW\")"
dd.BarManager.Shell.UsedBars(1).UsedActionObjs.Add(oMyActionObj)
dd.Barmanager.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Visible_ToActionObjCheckInt.htm`*

---
title: "ToActionObjCheckInt.OnClickCode"
description: "Specifies the VBS code that DIAdem executes when the bar element is clicked. Within the VBS code you can use and change the properties of the object. Use the Th"
---

# ToActionObjCheckInt.OnClickCode

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: OnClickCode for ActionObjCheckbutton

Specifies the VBS code that DIAdem executes when the bar element is clicked. Within the VBS code you can use and change the properties of the object. Use the This variable to access the object.

## Signature

```python
return_value = obj.OnClickCode
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can modify the <span class="Monospace">OnClickCode</span> property only for user-defined bar elements. The <a href="../toactionobjcheckint-kind/">Kind</a> property specifies whether a bar element is a free element or a user-defined element.</td>
</tr>
</table>
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If you use a <span class="Monospace">Refresh</span> method in the <span class="Monospace">OnClickCode</span> event, DIAdem does not refresh the display until the event has been executed.</td>
</tr>
</table>
<table class="Borderless" id="table6">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Do not implement your own <span class="Monospace">Function</span> or <span class="Monospace">Sub</span> procedure within the VBS code.</td>
</tr>
</table>
<table class="Borderless" id="table7">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You must not specify <span class="Monospace">Option Explicit</span> in the VBS code because DIAdem sets this statement implicitly.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oFloating = BarManager.ActionObjs.Add("PtlFloatingOnOff", "CustomCheckButton")
oFloating.Tooltip = "Floating Portal"
oFloatig.Picture  = "Portal.ico"
oFloating.OnRefreshCode.Code = "This.Check = PtlFloating"
oFloating.OnClickCode.Code = "PtlFloating = not This.Check"
BarManager.Bars("SCRMain").UsedActionObjs.Add(oFloating)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../methods/topropeventint-addcodeline/">AddCodeLine</a> | <a href="#" data-unresolved="1">Object Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_OnClickCode_ToActionObjCheckInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

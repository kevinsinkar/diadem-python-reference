---
title: "ToActionObjCheckInt.OnRefreshCode"
description: "Contains the VBS code of a button, which DIAdem executes during the refresh process. DIAdem executes a refresh, for example, when you switch a panel, open a bar"
---

# ToActionObjCheckInt.OnRefreshCode

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: OnRefreshCode for ActionObjCheckbutton

Contains the VBS code of a button, which DIAdem executes during the refresh process. DIAdem executes a refresh, for example, when you switch a panel, open a bar, or click a button. The refresh also executes if you specify a refresh command of the bar manager with a script. If the button is on one of the two bars that are always visible in a panel, you must execute the refresh. Within the VBS code you can use and change the properties of the object. Use the This variable to access the object.

## Signature

```python
return_value = obj.OnRefreshCode
```

## Notes

<div markdown="1">
<table class="Borderless" id="table3">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can modify the <span class="Monospace">OnRefreshCode</span> property only for user-defined bar elements. The <a href="../toactionobjcheckint-kind/">Kind</a> property specifies whether a bar element is a free element or a user-defined element.</td>
</tr>
</table>
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  A <span class="Monospace">Refresh</span> method cannot be called in the <span class="Monospace">OnRefreshCode</span> event.</td>
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
oFloating.Picture  = "Portal.ico"
oFloating.OnRefreshCode.Code = "This.Check = PtlFloating"
oFloating.OnClickCode.Code = "PtlFloating = not This.Check"
BarManager.Bars("SCRGroup").UsedActionObjs.Add(oFloating)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="../../methods/topropeventint-addcodeline/">AddCodeLine</a> | <a href="#" data-unresolved="1">Object Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_OnRefreshCode_ToActionObjCheckInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

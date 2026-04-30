---
title: "ToPropEventInt.Code"
description: "Specifies the VBS code of an event."
---

# ToPropEventInt.Code

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Code for Event

Specifies the VBS code of an event.

## Signature

```python
obj.Code
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>You can modify the <span class="Monospace">Code</span> property only for user-defined bar elements. The <span class="Monospace">Kind</span> property specifies whether a bar element is a free element or a user-defined element.</td>
</tr>
</table>
</div>

## Python example

```python
oActionObj = dd.BarManager.ActionObjs("MyCheckButton")
oActionObj.OnClickCode.Code = "Call MsgBoxDisp(\"Hello\")"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Code_ToPropEventInt.htm`*

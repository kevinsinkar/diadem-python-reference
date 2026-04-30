---
title: "ToBarManagerUIInt.FileName"
description: "Returns the name of the current bar definition. The filename extension is irrelevant. Note If you do not have your own bar definition, this property contains th"
---

# ToBarManagerUIInt.FileName

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: FileName for BarManager

Returns the name of the current bar definition. The filename extension is irrelevant. Note If you do not have your own bar definition, this property contains the name Desktop .

## Signature

```python
obj.FileName
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong> If you do not have your own bar definition, this property contains the name <span class="Monospace">Desktop</span>.</td>
</tr>
</table>
</div>

## Python example

```python
dd.MsgBoxDisp("Filename: " + dd.BarManager.FileName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_FileName_ToBarManagerUIInt.htm`*

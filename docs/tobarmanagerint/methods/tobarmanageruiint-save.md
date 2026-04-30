---
title: "ToBarManagerUIInt.Save"
description: "Overwrites the current bar definition if you do not specify a name for the bar definition, or saves the entire bar definition under a specified name. If you do "
---

# ToBarManagerUIInt.Save

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Save for BarManager

Overwrites the current bar definition if you do not specify a name for the bar definition, or saves the entire bar definition under a specified name. If you do not have your own bar definition and if you call the command without a file specification, DIAdem automatically generates a bar definition with the name of your desktop file, for example, Desktop.bdn , in the desktop folder. If the file is read only, DIAdem aborts the storage process with an error message. DIAdem overwrites existing files without a requesting confirmation.

## Signature

```python
bSave = Object.Save(FileName)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If you do not save the bar definition in the desktop folder or if you save it under a different name, you must load this bar definition at a later DIAdem start via the the <a href="../../objects/tobarmanageruiint/">BarManager</a> <a href="../tobarmanageruiint-load/">Load</a> method so that the bar definition impacts the DIAdem interface.</td>
</tr>
</table>
</div>

## Python example

```python
dd.BarManager.Save("MyDefinition.bdn")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Save_ToBarManagerUIInt.htm`*

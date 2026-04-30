---
title: "ToBarManagerInt.ResourcePath"
description: "Returns the path to the folder that contains the user-defined ICO files."
---

# ToBarManagerInt.ResourcePath

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: ResourcePath for BarManagerUnattached

Returns the path to the folder that contains the user-defined ICO files.

## Signature

```python
obj.ResourcePath
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If you do not save the bar definition in the desktop folder, the <a href="../../objects/tobarmanagerint/">BarManagerUnattached</a> <a href="../../methods/tobarmanagerint-save/">Save</a> method changes the <span class="Monospace">ResourcePath</span> property.</td>
</tr>
</table>
</div>

## Python example

```python
oMyBarUnattached = dd.BarManager.Create("")
oMyBarUnattached.Load("MyBar.bdn")
dd.MsgBoxDisp("Resource path: " + oMyBarUnattached.ResourcePath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_ResourcePath_ToBarManagerInt.htm`*

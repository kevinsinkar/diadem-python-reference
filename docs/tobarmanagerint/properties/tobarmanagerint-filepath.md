---
title: "ToBarManagerInt.FilePath"
description: "Returns the absolute path to the current bar definition of an additional bar manager, which is not used for the bar display in DIAdem. Note If you do not have y"
---

# ToBarManagerInt.FilePath

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: FilePath for BarManagerUnattached

Returns the absolute path to the current bar definition of an additional bar manager, which is not used for the bar display in DIAdem. Note If you do not have your own bar definition, this property contains the name of the desktop folder.

## Signature

```python
obj.FilePath
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  If you do not have your own bar definition, this property contains the name of the desktop folder.</td>
</tr>
</table>
</div>

## Python example

```python
oMyBarUnattached = dd.BarManager.Create("")
oMyBarUnattached.Load("MyBar.bdn")
dd.MsgBoxDisp("File path: " + oMyBarUnattached.FilePath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_FilePath_ToBarManagerInt.htm`*

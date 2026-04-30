---
title: "ToBarManagerInt.Save"
description: "Saves the entire bar definition of an additional bar manager, which is not used for the bar display in DIAdem, under a specified name. If the file is read only,"
---

# ToBarManagerInt.Save

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Save for BarManagerUnattached

Saves the entire bar definition of an additional bar manager, which is not used for the bar display in DIAdem, under a specified name. If the file is read only, DIAdem aborts the storage process with an error message. DIAdem overwrites existing files without a requesting confirmation.

## Signature

```python
bSave = Object.Save(FileName)
```

## Python example

```python
oMyBardef = dd.BarManager.Create("")
oMyBarDef.Import(dd.ConfReadPath + "Mybar.bdn",0)
oMyBarDef.Save("MyDefinition.bdn")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p><h2>Related Topics</h2><p><a href="../../../comoff/commands/executeexclusivebegin/">Command: ExecuteExclusiveBegin</a> | <a href="../../../comoff/commands/executeexclusiveend/">Command: ExecuteExclusiveEnd</a> | <a href="../../../comoff/commands/executeexclusiveendall/">Command: ExecuteExclusiveEndAll</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Save_ToBarManagerInt.htm`*

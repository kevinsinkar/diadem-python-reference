---
title: "ToBarManagerInt.CreateFromDeployment"
description: "Unpacks a Deployment file and generates a BarManagerUnattached object from the bar definition that is created. DIAdem saves the bar definition file that the Dep"
---

# ToBarManagerInt.CreateFromDeployment

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: CreateFromDeployment for BarManagerUnattached

Unpacks a Deployment file and generates a BarManagerUnattached object from the bar definition that is created. DIAdem saves the bar definition file that the Deployment contains in the target path with the respective subfolders and the ICO files that the subfolders contain. If you do not specify a target path, DIAdem saves the files in the user folder. The returned BarManager contains the unpacked and loaded bar definition.

## Signature

```python
return_value = obj.CreateFromDeployment(FileName, TargetPath)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  The file only can be unpacked if the target path does not contain a bar definition file and there is no subfolder with the same name.</td>
</tr>
</table>
</div>

## Python example

```python
oBarManager = dd.BarManager.CreateFromDeployment("MyBar.bdy","")
oBarManagerUnattached = oBarManager.Create("")
oBarManagerUnattached.Import(oBarManager,dd.eImportSkip)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_CreateFromDeployment_ToBarManagerInt.htm`*

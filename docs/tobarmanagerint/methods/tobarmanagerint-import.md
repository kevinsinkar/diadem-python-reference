---
title: "ToBarManagerInt.Import"
description: "Imports a bar definition to add bars and bar elements to the current bar definition. For the import of a bar definition the following rules apply: DIAdem only a"
---

# ToBarManagerInt.Import

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Import for BarManagerUnattached

Imports a bar definition to add bars and bar elements to the current bar definition. For the import of a bar definition the following rules apply: DIAdem only adds bars and bar elements. DIAdem does not delete bars or bar elements. DIAdem always adds the bar elements of a source bar to an identically-named target bar. DIAdem adds the bar element to the end of the bar. If the bar to be imported does not exist, DIAdem creates it. After importing the bar, DIAdem lists the imported bars and bar elements and any errors that might occur, in the logfile.

## Signature

```python
obj.Import(FileNameOrBarManager, Flag)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eImportAsk` | 0 | DIAdem asks whether to overwrite or to skip identically-named bar elements. |
| `eImportOverwrite` | 1 | DIAdem overwrites the identically-named bar element with the imported bar element. |
| `eImportSkip` | 2 | DIAdem skips the identically-named bar element, so that this element is not imported. |

## Python example

```python
oMyBardef = dd.BarManager.Create("")
oMyBarDef.Import(dd.ConfReadPath + "MyBarDef.bdn",dd.eImportSkip)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Import_ToBarManagerInt.htm`*

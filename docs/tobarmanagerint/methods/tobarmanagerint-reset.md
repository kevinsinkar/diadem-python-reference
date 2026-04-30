---
title: "ToBarManagerInt.Reset"
description: "Loads the original DIAdem bar definition and refreshes the bars."
---

# ToBarManagerInt.Reset

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Reset for BarManagerUnattached

Loads the original DIAdem bar definition and refreshes the bars.

## Signature

```python
obj.Reset
```

## Python example

```python
oMyBardef = dd.BarManager.Create("")
oMyBarDef.Import(dd.ConfReadPath + "Mybar.bdn",0)
oMyBarDef.Reset()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Reset_ToBarManagerInt.htm`*

---
title: "ToBarManagerInt.DataPortal"
description: "Returns the Data Portal."
---

# ToBarManagerInt.DataPortal

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: DataPortal for BarManagerUnattached

Returns the Data Portal.

## Signature

```python
return_value = obj.DataPortal
```

## Python example

```python
oMyBarManager = dd.BarManager.Create("")
for oMyBar in oMyBarManager.DataPortal.UsedBars:
    dd.MsgBoxDisp("Name: " + oMyBar.ID)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_DataPortal_ToBarManagerInt.htm`*

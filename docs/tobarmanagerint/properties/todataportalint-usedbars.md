---
title: "ToDataPortalInt.UsedBars"
description: "Returns a collection of all references to bars that the Data Portal contains."
---

# ToDataPortalInt.UsedBars

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: UsedBars for DataPortal

Returns a collection of all references to bars that the Data Portal contains.

## Signature

```python
return_value = obj.UsedBars
```

## Python example

```python
for oMyBar in dd.BarManager.DataPortal.UsedBars:
    dd.MsgBoxDisp("Name: " + oMyBar.ID)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_UsedBars_ToDataPortalInt.htm`*

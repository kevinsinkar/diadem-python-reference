---
title: "ToBarInt.ID"
description: "Returns the bar name, which is unique in the Bars collection."
---

# ToBarInt.ID

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: ID for Bar

Returns the bar name, which is unique in the Bars collection.

## Signature

```python
obj.ID
```

## Python example

```python
for oMyBar in dd.BarManager.Bars:
    i = i + 1
    dd.LogFileWrite(i + ", name of bar: " + oMyBar.ID)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_ID_ToBarInt.htm`*

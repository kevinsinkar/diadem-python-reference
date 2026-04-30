---
title: "ToBarManagerInt.Panels"
description: "Returns a collection of all panels that can contain bars for an additional bar manager. To access an individual panel in scripts, use the Item property, or ente"
---

# ToBarManagerInt.Panels

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Panels for BarManagerUnattached

Returns a collection of all panels that can contain bars for an additional bar manager. To access an individual panel in scripts, use the Item property, or enter the index or the name in parentheses.

## Signature

```python
return_value = obj.Panels
```

## Python example

```python
oMyBarManager = dd.BarManager.Create("")
for oMyPanel in oMyBarManager.Panels:
    dd.MsgBoxDisp("Name of panel: " + oMyPanel.ID)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Panels_ToBarManagerInt.htm`*

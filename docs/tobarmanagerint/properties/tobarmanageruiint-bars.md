---
title: "ToBarManagerUIInt.Bars"
description: "Returns a collection of all the bars that you can use in DIAdem. To access an individual bar in a script, use the Item property or enter the index or the name i"
---

# ToBarManagerUIInt.Bars

!!! abstract "Property &middot; `ToBarManagerInt.chm`"
    Property: Bars for BarManager

Returns a collection of all the bars that you can use in DIAdem. To access an individual bar in a script, use the Item property or enter the index or the name in parentheses.

## Signature

```python
return_value = obj.Bars
```

## Python example

```python
oMyBarUnattached = dd.BarManager.Create("")
dd.MsgBoxDisp("Number of bars: " + oMyBarUnattached.Bars.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/properties/DIABars_property_Bars_ToBarManagerUIInt.htm`*

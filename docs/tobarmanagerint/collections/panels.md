---
title: "Panels"
description: "A collection of all panels available in DIAdem. To access an individual panel in a script, use the Item method, or enter the index or the name in parentheses."
---

# Panels

!!! abstract "Collection &middot; `ToBarManagerInt.chm`"
    Collection: Panels

A collection of all panels available in DIAdem. To access an individual panel in a script, use the Item method, or enter the index or the name in parentheses.

## Python example

```python
for oMyBar in dd.BarManager.Panels("VIEW").UsedBars:
    dd.MsgBoxDisp("Name of bar: " + oMyBar.ID)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tomodulelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tomodulelistint-exists/">Exists</a> | <a href="../../methods/tomodulelistint-item/">Item</a> | <a href="../../methods/tomodulelistint-refresh/">Refresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/tobarmanageruiint/">BarManager</a>.<a href="../../properties/tobarmanageruiint-panels/">Panels</a> | <a href="../../objects/tobarmanagerint/">BarManagerUnattached</a>.<a href="../../properties/tobarmanagerint-panels/">Panels</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToModuleListInt.htm`*

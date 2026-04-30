---
title: "UsedBars"
description: "Collection of all bars used in a DIAdem panel or in the DIAdem main window. The bars that a panel or the DIAdem main window contain are references to bars of th"
---

# UsedBars

!!! abstract "Collection &middot; `ToBarManagerInt.chm`"
    Collection: UsedBars

Collection of all bars used in a DIAdem panel or in the DIAdem main window. The bars that a panel or the DIAdem main window contain are references to bars of the Bars collection. To access an individual bar in a script use the Item method or enter the index or the name in parentheses.

## Python example

```python
for oMyBar in dd.BarManager.Shell.UsedBars:
    dd.MsgBoxDisp("Name: " + oMyBar.ID)
```

```python
for oMyPanel in dd.BarManager.Panels:
    dd.MsgBoxDisp(oMyPanel.ID + ", " + oMyPanel.UsedBars.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tousedbarlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tousedbarlistint-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/todataportalint/">DataPortal</a>.<a href="../../properties/todataportalint-usedbars/">UsedBars</a> | <a href="../../objects/tomoduleint/">Panel</a>.<a href="../../properties/tomoduleint-usedbars/">UsedBars</a> | <a href="../../objects/toshellint/">Shell</a>.<a href="../../properties/toshellint-usedbars/">UsedBars</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToUsedBarListInt.htm`*

---
title: "Bars"
description: "Collection of all bars that you can use in DIAdem. To access an individual bar in a script use the Item method or enter the index or the name in parentheses."
---

# Bars

!!! abstract "Collection &middot; `ToBarManagerInt.chm`"
    Collection: Bars

Collection of all bars that you can use in DIAdem. To access an individual bar in a script use the Item method or enter the index or the name in parentheses.

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>If you press &lt;Shift-Ctrl&gt; and idle the cursor on a bar element, DIAdem displays a tooltip with the name of the bar, the name of the bar element, and the name of the base object, which is called the base type. DIAdem also copies this information, separated by a space, to the clipboard.</td>
</tr>
</table>
</div>

## Python example

```python
oMyActionObj = dd.BarManager.ActionObjs.Add("MyPopup", "CustomPopup")
oMyActionObj.Tooltip = "Opens MyBar"
dd.BarManager.Bars.Add("MyBar")
oMyActionObj.BarID = "MyBar"
dd.BarManager.Bars("SCRGroup").UsedActionObjs.Add(oMyActionObj)
```

```python
if dd.BarManager.Bars.Exists("MyBar") :
    dd.BarManager.Bars.Remove("MyBar")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tobarlistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tobarlistint-add/">Add</a> | <a href="../../methods/tobarlistint-exists/">Exists</a> | <a href="../../methods/tobarlistint-getuniqueid/">GetUniqueID</a> | <a href="../../methods/tobarlistint-item/">Item</a> | <a href="../../methods/tobarlistint-remove/">Remove</a> | <a href="../../methods/tobarlistint-removeall/">RemoveAll</a> | <a href="../../methods/tobarlistint-removeusedactionobj/">RemoveUsedActionObj</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/tobarmanageruiint/">BarManager</a>.<a href="../../properties/tobarmanageruiint-bars/">Bars</a> | <a href="../../objects/tobarmanagerint/">BarManagerUnattached</a>.<a href="../../properties/tobarmanagerint-bars/">Bars</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToBarListInt.htm`*

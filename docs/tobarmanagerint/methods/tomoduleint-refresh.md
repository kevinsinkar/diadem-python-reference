---
title: "ToModuleInt.Refresh"
description: "Rebuilds all the bars of a panel and refreshes the display."
---

# ToModuleInt.Refresh

!!! abstract "Method &middot; `ToBarManagerInt.chm`"
    Method: Refresh for Panel

Rebuilds all the bars of a panel and refreshes the display.

## Signature

```python
obj.Refresh
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note  </strong>The <span class="Monospace">Refresh</span> method cannot be called in the <span class="Monospace">OnRefreshCode</span> event.</td>
</tr>
</table>
</div>

## Python example

```python
dd.BarManager.Bars("SCRGroup").ActionObjPictureWidth = 18
dd.BarManager.Bars("SCRGroup").ActionObjPictureHeight = 18
BarManger.Panels("SCRIPT").Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/methods/DIABars_method_Refresh_ToModuleInt.htm`*

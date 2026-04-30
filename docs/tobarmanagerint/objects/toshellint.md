---
title: "ToShellInt"
description: "The Shell object provides the DIAdem main window that can contain bars like a DIAdem panel. Note If you press <Shift-Ctrl> and idle the cursor on a bar element,"
---

# ToShellInt

!!! abstract "Object &middot; `ToBarManagerInt.chm`"
    Object: Shell

The Shell object provides the DIAdem main window that can contain bars like a DIAdem panel. Note If you press <Shift-Ctrl> and idle the cursor on a bar element, DIAdem displays a tooltip with the name of the bar, the name of the bar element, and the name of the base object, which is called the base type. DIAdem also copies this information, separated by a space, to the clipboard.

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
for oMyBar in dd.BarManager.Shell.UsedBars:
    dd.MsgBoxDisp("Name: " + oMyBar.ID)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/toshellint-usedbars/">UsedBars</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../tobarmanageruiint/">BarManager</a>.<a href="../../properties/tobarmanageruiint-shell/">Shell</a> | <a href="../tobarmanagerint/">BarManagerUnattached</a>.<a href="../../properties/tobarmanagerint-shell/">Shell</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Adding User-Defined Functions to the Group Bar</a> | <a href="#" data-unresolved="1">Creating and Saving a Work Session</a> | <a href="#" data-unresolved="1">Custom Toolbars on DIAdem Panels</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Merge Bar Definitions</a> | <a href="#" data-unresolved="1">User-Defined Evaluations in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">User-Defined Menus</a> | <a href="#" data-unresolved="1">Working with the Bar Manager</a></p>
</div>
</div>

---

*Source: `ToBarManagerInt/objects/DIABars_Objects_ToShellInt.htm`*

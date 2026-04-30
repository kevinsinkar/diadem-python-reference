---
title: "VIEW.Refresh"
description: "Refreshes the layout in DIAdem VIEW. DIAdem checks whether the displayed data has changed."
---

# VIEW.Refresh

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: Refresh for View

Refreshes the layout in DIAdem VIEW. DIAdem checks whether the displayed data has changed.

## Signature

```python
obj.Refresh()
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  If the <a href="../../properties/view-autorefresh/">AutoRefresh</a> property is <span class="Monospace">FALSE</span>, the <span class="Monospace">Refresh</span> method is not effective.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  If a script modifies the properties or the contents of data channels, set the <a href="../../properties/view-autorefresh/">AutoRefresh</a> property to <span class="Monospace">FALSE</span> to speed up the script. You then call the <span class="Monospace">Refresh</span> method to refresh the values displayed in DIAdem VIEW.</td></tr></table>
</div>

## Python example

```python
dd.View.AutoRefresh = True
dd.View.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_Refresh_VIEW.htm`*

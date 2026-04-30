---
title: "VIEW.AutoRefresh"
description: "Specifies whether DIAdem refreshes the layout in DIAdem VIEW."
---

# VIEW.AutoRefresh

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: AutoRefresh for View

Specifies whether DIAdem refreshes the layout in DIAdem VIEW.

## Signature

```python
obj.AutoRefresh
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  If a script modifies the properties or the contents of data channels, set the <span class="Monospace">AutoRefresh</span> property to <span class="Monospace">FALSE</span> to speed up the script. You then call the <a href="../../methods/view-refresh/">Refresh</a> method to refresh the values displayed in DIAdem VIEW.</td></tr></table>
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

*Source: `Scriptview/properties/VIEW_property_AutoRefresh_VIEW.htm`*

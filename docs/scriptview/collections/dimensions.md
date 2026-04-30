---
title: "Dimensions"
description: "The Dimension object provides a collection of all Dimensions in DIAdem VIEW. Use the Dimensions collection to delete the Cursor dimensions or to add a new Curso"
---

# Dimensions

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Dimensions

The Dimension object provides a collection of all Dimensions in DIAdem VIEW. Use the Dimensions collection to delete the Cursor dimensions or to add a new Cursor dimension.

## Python example

```python
for oMyDim in dd.View.ActiveSheet.Cursor.Dimensions:
    dd.MsgBoxDisp(oMyDim.Name + " / " + oMyDim.Type)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itodimensionsint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itodimensionsint-add/">Add</a> | <a href="../../methods/itodimensionsint-exists/">Exists</a> | <a href="../../methods/itodimensionsint-item/">Item</a> | <a href="../../methods/itodimensionsint-remove/">Remove</a> | <a href="../../methods/itodimensionsint-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToDimensionsInt.htm`*

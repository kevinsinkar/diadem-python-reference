---
title: "IToDimensionInt"
description: "The Dimension object provides a cursor dimension in DIAdem VIEW."
---

# IToDimensionInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Dimension

The Dimension object provides a cursor dimension in DIAdem VIEW.

## Python example

```python
for oMyDim in dd.View.ActiveSheet.Cursor.Dimensions:
    dd.MsgBoxDisp(oMyDim.Name + " / " + oMyDim.Type)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itodimensionint-description/">Description</a> | <a href="../../properties/itodimensionint-difference/">Difference</a> | <a href="../../properties/itodimensionint-index/">Index</a> | <a href="../../properties/itodimensionint-name/">Name</a> | <a href="../../properties/itodimensionint-type/">Type</a> | <a href="../../properties/itodimensionint-value1/">Value1</a> | <a href="../../properties/itodimensionint-value2/">Value2</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/dimensions/">Dimensions</a>.<a href="../../methods/itodimensionsint-add/">Add</a> | <a href="../../collections/dimensions/">Dimensions</a>.<a href="../../methods/itodimensionsint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToDimensionInt.htm`*

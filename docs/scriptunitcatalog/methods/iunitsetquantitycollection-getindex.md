---
title: "IUnitSetQuantityCollection.GetIndex"
description: "Returns the index of a physical quantity that is used, from a unit set in the units catalog."
---

# IUnitSetQuantityCollection.GetIndex

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: GetIndex for UsedQuantities

Returns the index of a physical quantity that is used, from a unit set in the units catalog.

## Signature

```python
iGetIndex = Object.GetIndex(Name)
```

## Python example

```python
iGetIndex = dd.UnitCatalog.Sets("mechanics").UsedQuantities.GetIndex("volume")
dd.MsgBoxDisp(dd.UnitCatalog.Sets("mechanics").UsedQuantities(iGetIndex).name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_GetIndex_IUnitSetQuantityCollection.htm`*

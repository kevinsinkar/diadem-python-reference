---
title: "IUnitSetQuantityCollection.Move"
description: "Changes the position of a physical quantity in the UsedQuantities collection in the units catalog. If you change the position, you also change the index of the "
---

# IUnitSetQuantityCollection.Move

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: Move for UsedQuantities

Changes the position of a physical quantity in the UsedQuantities collection in the units catalog. If you change the position, you also change the index of the physical quantity.

## Signature

```python
obj.Move(FromPosition, ToPosition)
```

## Python example

```python
dd.UnitCatalog.Sets("mechanics").UsedQuantities.Move(1,3)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_Move_IUnitSetQuantityCollection.htm`*

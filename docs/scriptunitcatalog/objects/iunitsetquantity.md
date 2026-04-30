---
title: "IUnitSetQuantity"
description: "The UsedQuantity object specifies a physical quantity that is used in a unit set of the units catalog."
---

# IUnitSetQuantity

!!! abstract "Object &middot; `ScriptUnitCatalog.chm`"
    Object: UsedQuantity

The UsedQuantity object specifies a physical quantity that is used in a unit set of the units catalog.

## Python example

```python
oMyUsedQuantity = dd.UnitCatalog.Sets(1).UsedQuantities(1)
dd.MsgBoxDisp(dd.UnitCatalog.Quantities(oMyUsedQuantity.Name).DisplayName)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iunitsetquantity-defaultunit/">DefaultUnit</a> | <a href="../../properties/iunitsetquantity-name/">Name</a> | <a href="../../properties/iunitsetquantity-usedunits/">UsedUnits</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/usedquantities/">UsedQuantities</a>.<a href="../../methods/iunitsetquantitycollection-add/">Add</a> | <a href="../../collections/usedquantities/">UsedQuantities</a>.<a href="../../methods/iunitsetquantitycollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/objects/DiaCmpnt_Objects_IUnitSetQuantity.htm`*

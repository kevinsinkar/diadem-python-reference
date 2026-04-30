---
title: "UsedUnits"
description: "The UsedUnits collection provides all the units of a physical quantity that are used, from a specific unit set in the units catalog."
---

# UsedUnits

!!! abstract "Collection &middot; `ScriptUnitCatalog.chm`"
    Collection: UsedUnits

The UsedUnits collection provides all the units of a physical quantity that are used, from a specific unit set in the units catalog.

## Python example

```python
for oMyUnit in dd.UnitCatalog.Sets("mechanics").UsedQuantities("length").UsedUnits:
    sOutput = sOutput + oMyUnit.Name + "\r\n"
dd.MsgBoxDisp (sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iunitsetunitcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iunitsetunitcollection-add/">Add</a> | <a href="../../methods/iunitsetunitcollection-exists/">Exists</a> | <a href="../../methods/iunitsetunitcollection-getindex/">GetIndex</a> | <a href="../../methods/iunitsetunitcollection-item/">Item</a> | <a href="../../methods/iunitsetunitcollection-move/">Move</a> | <a href="../../methods/iunitsetunitcollection-remove/">Remove</a> | <a href="../../methods/iunitsetunitcollection-setasdefault/">SetAsDefault</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/iunitsetquantity/">UsedQuantity</a>.<a href="../../properties/iunitsetquantity-usedunits/">UsedUnits</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/objects/DiaCmpnt_Objects_IUnitSetUnitCollection.htm`*

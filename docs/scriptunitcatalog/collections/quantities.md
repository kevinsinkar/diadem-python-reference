---
title: "Quantities"
description: "The Quantities collection provides all the physical quantities from the units catalog."
---

# Quantities

!!! abstract "Collection &middot; `ScriptUnitCatalog.chm`"
    Collection: Quantities

The Quantities collection provides all the physical quantities from the units catalog.

## Python example

```python
for oMyQuantity in dd.UnitCatalog.Quantities:
    sOutput = sOutput + oMyQuantity.Name +"\r\n"
dd.MsgBoxdisp (sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iphysicalquantitycollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iphysicalquantitycollection-add/">Add</a> | <a href="../../methods/iphysicalquantitycollection-exists/">Exists</a> | <a href="../../methods/iphysicalquantitycollection-getindex/">GetIndex</a> | <a href="../../methods/iphysicalquantitycollection-item/">Item</a> | <a href="../../methods/iphysicalquantitycollection-move/">Move</a> | <a href="../../methods/iphysicalquantitycollection-remove/">Remove</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/iunitcatalog/">UnitCatalog</a>.<a href="../../properties/iunitcatalog-quantities/">Quantities</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/objects/DiaCmpnt_Objects_IPhysicalQuantityCollection.htm`*

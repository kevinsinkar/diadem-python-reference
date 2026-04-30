---
title: "Sets"
description: "The Sets collection provides all the unit sets of the units catalog."
---

# Sets

!!! abstract "Collection &middot; `ScriptUnitCatalog.chm`"
    Collection: Sets

The Sets collection provides all the unit sets of the units catalog.

## Python example

```python
for oMySet in dd.UnitCatalog.Sets:
    sOutput = sOutput + oMySet.Name + "\r\n"
dd.MsgBoxDisp (sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iunitsetcollection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iunitsetcollection-add/">Add</a> | <a href="../../methods/iunitsetcollection-exists/">Exists</a> | <a href="../../methods/iunitsetcollection-getindex/">GetIndex</a> | <a href="../../methods/iunitsetcollection-item/">Item</a> | <a href="../../methods/iunitsetcollection-move/">Move</a> | <a href="../../methods/iunitsetcollection-remove/">Remove</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/iunitcatalog/">UnitCatalog</a>.<a href="../../properties/iunitcatalog-sets/">Sets</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/objects/DiaCmpnt_Objects_IUnitSetCollection.htm`*

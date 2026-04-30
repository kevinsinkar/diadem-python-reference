---
title: "IUnitSymbol"
description: "The Symbol object specifies the symbol of a unit from a unit set in the units catalog."
---

# IUnitSymbol

!!! abstract "Object &middot; `ScriptUnitCatalog.chm`"
    Object: Symbol

The Symbol object specifies the symbol of a unit from a unit set in the units catalog.

## Python example

```python
dd.MsgBoxDisp (dd.UnitCatalog.Sets("mechanics").UsedQuantities("length").UsedUnits("meter").Symbol.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iunitsymbol-description/">Description</a> | <a href="../../properties/iunitsymbol-name/">Name</a> | <a href="../../properties/iunitsymbol-unit/">Unit</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iunitsymbol-activate/">Activate</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/allsymbols/">AllSymbols</a>.<a href="../../methods/iunitcatalogsymbolcollection-item/">Item</a> | <a href="../../collections/symbolaliases/">SymbolAliases</a>.<a href="../../methods/iunitsymbolcollection-add/">Add</a> | <a href="../../collections/symbolaliases/">SymbolAliases</a>.<a href="../../methods/iunitsymbolcollection-item/">Item</a> | <a href="../iphysicalunit/">Unit</a>.<a href="../../properties/iphysicalunit-symbol/">Symbol</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/objects/DiaCmpnt_Objects_IUnitSymbol.htm`*

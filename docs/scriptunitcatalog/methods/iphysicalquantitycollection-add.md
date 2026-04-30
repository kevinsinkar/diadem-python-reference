---
title: "IPhysicalQuantityCollection.Add"
description: "Adds a physical quantity to the units catalog."
---

# IPhysicalQuantityCollection.Add

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: Add for Quantities

Adds a physical quantity to the units catalog.

## Signature

```python
return_value = obj.Add(Name, LengthExp, MassExp, TimeExp, CurrentExp, TemperatureExp, MolarAmountExp, LuminousIntensityExp)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The parameters <em>LengthExp</em>, <em>MassExp</em>, <em>TimeExp</em>, <em>CurrentExp</em>, <em>TemperatureExp</em>, <em>MolarAmountExp</em>, and <em>LuminousIntensityExp</em> specify the <a href="#" data-unresolved="1">Dimension</a> of a physical quantity.</td></tr></table>
</div>

## Python example

```python
dd.UnitCatalog.Quantities.Add("NewQuantity",1,0,0,0,0,0,0)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_Add_IPhysicalQuantityCollection.htm`*

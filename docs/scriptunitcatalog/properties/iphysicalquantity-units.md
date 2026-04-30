---
title: "IPhysicalQuantity.Units"
description: "Returns the collection of all the units of a physical quantity in the units catalog."
---

# IPhysicalQuantity.Units

!!! abstract "Property &middot; `ScriptUnitCatalog.chm`"
    Property: Units for Quantity

Returns the collection of all the units of a physical quantity in the units catalog.

## Signature

```python
return_value = obj.Units
```

## Python example

```python
for oMyUnit in dd.UnitCatalog.Quantities("time").Units:
    sOutput = sOutput + oMyUnit.Name + "\r\n"
dd.MsgBoxDisp (sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/properties/DiaCmpnt_property_Units_IPhysicalQuantity.htm`*

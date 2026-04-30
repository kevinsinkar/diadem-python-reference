---
title: "IUnitSetQuantityCollection.Add"
description: "Adds a physical quantity to a unit set, in the units catalog."
---

# IUnitSetQuantityCollection.Add

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: Add for UsedQuantities

Adds a physical quantity to a unit set, in the units catalog.

## Signature

```python
return_value = obj.Add(Name)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table2"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You only can add a physical quantity that already exists in the units catalog, to a unit set.</td></tr></table>
</div>

## Python example

```python
dd.UnitCatalog.Sets("Custom").UsedQuantities.Add("temperature")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_Add_IUnitSetQuantityCollection.htm`*

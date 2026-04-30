---
title: "IUnitCatalog.Modified"
description: "Indicates whether the units catalog has been modified since the last time the DIAdem settings were changed. If the units catalog has been modified, the Modified"
---

# IUnitCatalog.Modified

!!! abstract "Property &middot; `ScriptUnitCatalog.chm`"
    Property: Modified for UnitCatalog

Indicates whether the units catalog has been modified since the last time the DIAdem settings were changed. If the units catalog has been modified, the Modified property is TRUE, otherwise the property is FALSE.

## Signature

```python
obj.Modified
```

## Python example

```python
if not dd.UnitCatalog.Quantities.Exists("NewQuantity") :
    dd.UnitCatalog.Quantities.Add("NewQuantity",1,1,1,1,1,1,1)
    dd.LogfileWrite("UnitCatalog modified: " + dd.UnitCatalog.Modified) #TRUE
    if dd.UnitCatalog.Modified :
        dd.UnitCatalog.ResetModified()
    dd.LogfileWrite("UnitCatalog modified: " + dd.UnitCatalog.Modified) #FALSE
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/properties/DiaCmpnt_property_Modified_IUnitCatalog.htm`*

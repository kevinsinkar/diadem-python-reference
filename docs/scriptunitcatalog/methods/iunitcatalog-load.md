---
title: "IUnitCatalog.Load"
description: "Loads the contents of a units catalog from a file with the filename extension *.tuc . DIAdem overwrites existing contents. The UnitCatalog object is available a"
---

# IUnitCatalog.Load

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: Load for UnitCatalog

Loads the contents of a units catalog from a file with the filename extension *.tuc . DIAdem overwrites existing contents. The UnitCatalog object is available as a global object in scripts and in dialog boxes. If you want to prepare further catalog units without changing the loaded units catalog, use the OpenExternalCatalog method.

## Signature

```python
obj.Load(FileName)
```

## Python example

```python
dd.UnitCatalog.Load("C:\\MyUnits.tuc")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_Load_IUnitCatalog.htm`*

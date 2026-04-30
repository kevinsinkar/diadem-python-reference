---
title: "IUnitCatalog.OpenExternalCatalog"
description: "Opens an external units catalog in DIAdem. This units catalog is only available in a script and does not influence the standard units catalog or the dialog boxe"
---

# IUnitCatalog.OpenExternalCatalog

!!! abstract "Method &middot; `ScriptUnitCatalog.chm`"
    Method: OpenExternalCatalog for UnitCatalog

Opens an external units catalog in DIAdem. This units catalog is only available in a script and does not influence the standard units catalog or the dialog boxes in DIAdem. You can use it to prepare further units catalogs, then save it with the method SaveAs , and load it with the method Load , in order to make it available as a global object in scripts and dialog boxes.

## Signature

```python
return_value = obj.OpenExternalCatalog(FileName)
```

## Python example

```python
oMyCatalog = dd.UnitCatalog.OpenExternalCatalog(dd.ScriptReadPath + "MyCatalog.tuc")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a> | <a href="../iunitcatalog-saveas/">SaveAs</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Adding an Unknown Unit Symbol to the Units Catalog</a> | <a href="#" data-unresolved="1">Converting Channel Units in DIAdem ANALYSIS</a> | <a href="#" data-unresolved="1">Converting Channel Units with a Script</a> | <a href="#" data-unresolved="1">Converting Channels According to a Unit Set</a> | <a href="#" data-unresolved="1">Creating a New Unit Set</a> | <a href="#" data-unresolved="1">Creating a Physical Quantity in the Units Catalog</a> | <a href="#" data-unresolved="1">Extending the Units Catalog with a Script</a> | <a href="#" data-unresolved="1">Replacing and Converting Channel Units in the Input Help</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Converting Units</a></p>
</div>
</div>

---

*Source: `ScriptUnitCatalog/methods/DiaCmpnt_method_OpenExternalCatalog_IUnitCatalog.htm`*

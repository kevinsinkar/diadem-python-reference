---
title: "IDocumentNamespace.Properties"
description: "Returns all meta properties in a specific namespace of a document. Use namespaces to identify XML elements clearly in a document."
---

# IDocumentNamespace.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for DocumentNamespace <DataPlugin>

Returns all meta properties in a specific namespace of a document. Use namespaces to identify XML elements clearly in a document.

## Signature

```python
return_value = obj.Properties
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyNamespace in Document.Namespaces:
    for oMyProp in oMyNamespace.Properties:
        Root.Properties.Add(oMyProp.Name, oMyProp.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IDocumentNamespace.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

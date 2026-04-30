---
title: "IDocumentRoot.Namespaces"
description: "Returns all namespaces of a document. Use namespaces to identify groups of XML elements in a document."
---

# IDocumentRoot.Namespaces

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Namespaces for Document <DataPlugin>

Returns all namespaces of a document. Use namespaces to identify groups of XML elements in a document.

## Signature

```python
return_value = obj.Namespaces
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

*Source: `DataPlugin/Properties/DataPlugin_property_Namespaces_IDocumentRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IDocumentNamespace.Name"
description: "Returns the name of a namespace in a document. Use namespaces to group XML elements in a document."
---

# IDocumentNamespace.Name

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Name for DocumentNamespace <DataPlugin>

Returns the name of a namespace in a document. Use namespaces to group XML elements in a document.

## Signature

```python
obj.Name
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyNamespace in Document.Namespaces:
    Root.Properties.Add(oMyNamespace.Name, oMyNamespace.Properties.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Name_IDocumentNamespace.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IDocumentProperty.Custom"
description: "Specifies whether a meta property of a document is a custom property. Custom properties are user-defined meta properties of a document. A document can be an Off"
---

# IDocumentProperty.Custom

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Custom for DocumentProperty <DataPlugin>

Specifies whether a meta property of a document is a custom property. Custom properties are user-defined meta properties of a document. A document can be an Office file in XML format, a PDF, JPEG, PNG, or TIFF file.

## Signature

```python
obj.Custom
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProp in Document.Properties:
    if oMypPop.Custom:
        Root.Properties.Add("Custom_"&oMyProp.Name, oMyProp.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Custom_IDocumentProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IDocumentProperty"
description: "The DocumentProperty <DataPlugin> object provides a document's meta property. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file"
---

# IDocumentProperty

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: DocumentProperty <DataPlugin>

The DocumentProperty <DataPlugin> object provides a document's meta property. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProperty in Document.Properties:
    Root.Properties.Add(oMyProperty.Name, oMyProperty.Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idocumentproperty-custom/">Custom</a> | <a href="../../properties/idocumentproperty-datatype/">DataType</a> | <a href="../../properties/idocumentproperty-name/">Name</a> | <a href="../../properties/idocumentproperty-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/documentproperties/">DocumentProperties &lt;DataPlugin&gt;</a>.<a href="../../methods/idocumentreadproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IDocumentProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

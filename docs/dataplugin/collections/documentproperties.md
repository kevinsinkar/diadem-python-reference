---
title: "DocumentProperties"
description: "Collection of a document's meta properties not allocated to any namespace. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file."
---

# DocumentProperties

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: DocumentProperties <DataPlugin>

Collection of a document's meta properties not allocated to any namespace. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file.

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
<p><a href="../../properties/idocumentreadproperties-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idocumentreadproperties-exists/">Exists</a> | <a href="../../methods/idocumentreadproperties-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idocumentroot/">Document &lt;DataPlugin&gt;</a>.<a href="../../properties/idocumentroot-properties/">Properties</a> | <a href="../../objects/idocumentnamespace/">DocumentNamespace &lt;DataPlugin&gt;</a>.<a href="../../properties/idocumentnamespace-properties/">Properties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IDocumentReadProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

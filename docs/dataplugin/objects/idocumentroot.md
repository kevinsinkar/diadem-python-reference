---
title: "IDocumentRoot"
description: "The Document <DataPlugin> object provides the properties and methods for accessing the meta properties of a document. A document might be an Office file in XML "
---

# IDocumentRoot

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Document <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The Document <DataPlugin> object provides the properties and methods for accessing the meta properties of a document. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file.

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
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/idocumentroot-filepath/">FilePath</a> | <a href="../../properties/idocumentroot-filetype/">FileType</a> | <a href="../../properties/idocumentroot-namespaces/">Namespaces</a> | <a href="../../properties/idocumentroot-properties/">Properties</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idataplugin/">DataPlugin</a>.<a href="../../methods/idataplugin-opendocument/">OpenDocument</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IDocumentRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IDocumentProperty.Value"
description: "Specifies the value of a meta property of a document.  A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file."
---

# IDocumentProperty.Value

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Value for DocumentProperty <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the value of a meta property of a document.  A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file.

## Signature

```python
obj.Value
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProperty in Document.Properties:
    Root.Properties.Add(oMyProperty.Name, oMyProperty.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Value_IDocumentProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IDocumentNamespaces.Count"
description: "Returns the number of namespaces of a document. Use namespaces to group XML elements in a document."
---

# IDocumentNamespaces.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for DocumentNamespaces <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the number of namespaces of a document. Use namespaces to group XML elements in a document.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, Document.Namespaces.Count + 1):
    oMyNameSpaceProps = Document.Namespaces(i).Properties
    for j in range(1, oMyNameSpaceProps.Count + 1):
        Root.Properties.Add(oMyNameSpaceProps(j).Name, oMyNameSpaceProps(j).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IDocumentNamespaces.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

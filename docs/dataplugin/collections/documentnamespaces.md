---
title: "DocumentNamespaces"
description: "Collection of name spaces in a document. Use namespaces to group XML elements in a document."
---

# DocumentNamespaces

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: DocumentNamespaces <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Collection of name spaces in a document. Use namespaces to group XML elements in a document.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyNameSpace in Document.Namespaces:
    for oMyProperty in oMyNameSpace.Properties:
        Root.Properties.Add(oMyProperty.Name, oMyProperty.Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idocumentnamespaces-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idocumentnamespaces-exists/">Exists</a> | <a href="../../methods/idocumentnamespaces-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idocumentroot/">Document &lt;DataPlugin&gt;</a>.<a href="../../properties/idocumentroot-namespaces/">Namespaces</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IDocumentNamespaces.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

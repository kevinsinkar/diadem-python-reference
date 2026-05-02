---
title: "IDocumentNamespaces.Item"
description: "Returns a namespace of a document. Use namespaces to group XML elements in a document."
---

# IDocumentNamespaces.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for DocumentNamespaces <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns a namespace of a document. Use namespaces to group XML elements in a document.

## Signature

```python
return_value = obj.Item(PropNameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img src="../image/note.gif"/></td>
<td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, Document.Namespaces.Count + 1):
    oMyNamespaceProps = Document.Namespaces(i).Properties
    for j in range(1, oMyNamespaceProps.Count + 1):
        Root.Properties.Add(oMyNamespaceProps(j).Name, oMyNamespaceProps(j).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IDocumentNamespaces.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

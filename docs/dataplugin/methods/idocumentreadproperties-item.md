---
title: "IDocumentReadProperties.Item"
description: "Returns a document's meta property not allocated to a namespace. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file."
---

# IDocumentReadProperties.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for DocumentProperties <DataPlugin>

Returns a document's meta property not allocated to a namespace. A document might be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file.

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
oMyProperties = Document.Properties
for i in range(1, oMyProperties.Count + 1):
    Root.Properties.Add(oMyProperties(i).Name, oMyProperties(i).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IDocumentReadProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

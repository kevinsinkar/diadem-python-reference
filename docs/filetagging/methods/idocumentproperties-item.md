---
title: "IDocumentProperties.Item"
description: "Returns a changeable meta property that is not assigned to a namespace, from the top level of a document. A document may be an Office file in XML format or a PD"
---

# IDocumentProperties.Item

!!! abstract "Method &middot; `FileTagging.chm`"
    Method: Item for DocumentProperties <Data>

Returns a changeable meta property that is not assigned to a namespace, from the top level of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
for iCount in range( 1, oMyDocument.Properties.Count+1):
    sOut = sOut + "Name: " + oMyDocument.Properties(iCount).Name + ", Value: " + oMyDocument.Properties(iCount).Value  + "\r\n"
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/methods/DiaCmpnt_method_Item_IDocumentProperties.htm`*

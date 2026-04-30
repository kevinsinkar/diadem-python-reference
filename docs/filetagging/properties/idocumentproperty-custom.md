---
title: "IDocumentProperty.Custom"
description: "Specifies whether a meta property of a document is a custom property. Custom properties are user-defined meta properties from the top level of a document. You c"
---

# IDocumentProperty.Custom

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: Custom for DocumentProperty <Data>

Specifies whether a meta property of a document is a custom property. Custom properties are user-defined meta properties from the top level of a document. You can read, create, edit, and delete custom properties. You can only read the other meta properties of a document and edit their values. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.Custom
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
sOut = "File path: " + oMyDocument.FilePath + "\r\n"
for oMyProperty in oMyDocument.Properties:
    if oMyProperty.Custom :
        sOut = sOut + "Name: " + oMyProperty.Name + ", Value: " + oMyProperty.Value  + "\r\n"
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/properties/DiaCmpnt_property_Custom_IDocumentProperty.htm`*

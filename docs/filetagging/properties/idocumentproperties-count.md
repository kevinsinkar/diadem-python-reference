---
title: "IDocumentProperties.Count"
description: "Returns the number of meta properties of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the O"
---

# IDocumentProperties.Count

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: Count for DocumentProperties <Data>

Returns the number of meta properties of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
sOut = "Number of properties: " + oMyDocument.Properties.Count + "\r\n"
for oMyProperty in oMyDocument.Properties:
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

*Source: `FileTagging/properties/DiaCmpnt_property_Count_IDocumentProperties.htm`*

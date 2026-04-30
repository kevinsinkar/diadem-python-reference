---
title: "IDiademDocument.ReadOnly"
description: "Specifies whether a document was opened in read-only mode. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use"
---

# IDiademDocument.ReadOnly

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: ReadOnly for Document <Data>

Specifies whether a document was opened in read-only mode. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.ReadOnly
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
if not(oMyDocument.ReadOnly) :
    oMyDocument.Properties.Add("Modified","Yes", dd.DataTypeDocumentString)
sOut = "File path: " + oMyDocument.FilePath + "\r\n"
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

*Source: `FileTagging/properties/DiaCmpnt_property_ReadOnly_IDiademDocument.htm`*

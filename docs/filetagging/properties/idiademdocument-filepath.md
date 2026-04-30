---
title: "IDiademDocument.FilePath"
description: "Returns the absolute path of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument "
---

# IDiademDocument.FilePath

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: FilePath for Document <Data>

Returns the absolute path of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.FilePath
```

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
sOut = "File path: " + oMyDocument.FilePath
print(sOut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/properties/DiaCmpnt_property_FilePath_IDiademDocument.htm`*

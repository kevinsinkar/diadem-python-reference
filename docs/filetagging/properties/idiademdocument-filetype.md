---
title: "IDiademDocument.FileType"
description: "Returns the data type of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument comm"
---

# IDiademDocument.FileType

!!! abstract "Property &middot; `FileTagging.chm`"
    Property: FileType for Document <Data>

Returns the data type of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP. Use the OpenDocument command to open a document.

## Signature

```python
obj.FileType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDocumentTypeAuto` | 0 | The file type is specified automatically from the filename extension. DIAdem does not return this file type but always one of the following. |
| `eDocumentTypeXMP` | 1 | XMP file (for example *.pdf; *.jpg; *.jpeg; *.png; *.tif; *.tiff) |
| `eDocumentTypeWord` | 2 | XML based Word file (for example *.docx; *.docm; *.dotx; *.dotm) |
| `eDocumentTypeExcel` | 3 | XML based Excel file (for example *.xlsx; *.xltm; *.xltx; *.xltm) |
| `eDocumentTypePowerPoint` | 4 | XML based PowerPoint file (for example *.pptx; *.pptm; *.potx; *.potm) |

## Python example

```python
oMyDocument = dd.OpenDocument(dd.ProgramDrv + "Manuals\\DIAdem_GettingStarted.pdf", False, dd.eDocumentTypeAuto)
sOut = "File type: " + sFileType(oMyDocument.FileType)
print(sOut)

def sFileType(iFileType):
    select_variable_0 = iFileType
    if (select_variable_0 == dd.eDocumentTypeXMP) :
        sFileType = "XMP"
    elif (select_variable_0 == dd.eDocumentTypeWord) :
        sFileType = "Word"
    elif (select_variable_0 == dd.eDocumentTypeExcel) :
        sFileType = "Excel"
    elif (select_variable_0 == dd.eDocumentTypePowerPoint) :
        sFileType = "PowerPoint"
    return sFileType
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `FileTagging/properties/DiaCmpnt_property_FileType_IDiademDocument.htm`*

---
title: "IDataPlugin.OpenDocument"
description: "Returns an object which provides methods and properties for reading or editing the metadata of a document."
---

# IDataPlugin.OpenDocument

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: OpenDocument for DataPlugin

Returns an object which provides methods and properties for reading or editing the metadata of a document.

## Signature

```python
return_value = obj.OpenDocument(FileName, DocumentType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDocumentTypeAuto` | 0 | The file type is specified automatically from the filename extension |
| `eDocumentTypeXMP` | 1 | XMPfile (for example *.pdf; *.jpg; *.jpeg; *.png; *.tif; *.tiff) |
| `eDocumentTypeWord` | 2 | XML based Word file (for example *.docx; *.docm; *.dotx; *.dotm) |
| `eDocumentTypeExcel` | 3 | XML based Excel file (for example *.xlsx; *.xltm; *.xltx; *.xltm) |
| `eDocumentTypePowerPoint` | 4 | XML based PowerPoint file (for example *.pptx; *.pptm; *.potx; *.potm) |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyDocument = OpenDocument("c:\test.pdf", eDocumentTypeAuto)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_OpenDocument_IDataPlugin.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IDocumentRoot.FileType"
description: "Returns the data type of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP."
---

# IDocumentRoot.FileType

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: FileType for Document <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the data type of a document. A document may be an Office file in XML format or a PDF, JPEG, PNG, or TIFF file, which uses XMP.

## Signature

```python
obj.FileType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDocumentTypeXMP` | 1 | XMP file (for example *.pdf; *.jpg; *.jpeg; *.png; *.tif; *.tiff) |
| `eDocumentTypeWord` | 2 | XML based Word file (for example *.docx; *.docm; *.dotx; *.dotm) |
| `eDocumentTypeExcel` | 3 | XML based Excel file (for example *.xlsx; *.xltm; *.xltx; *.xltm) |
| `eDocumentTypePowerPoint` | 4 | XML based PowerPoint file (for example *.pptx; *.pptm; *.potx; *.potm) |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("DocumentFileType",Document.FileType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_FileType_IDocumentRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

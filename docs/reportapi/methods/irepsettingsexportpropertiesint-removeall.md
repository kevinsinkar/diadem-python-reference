---
title: "IRepSettingsExportPropertiesInt.RemoveAll"
description: "Deletes all custom properties in DIAdem REPORT for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG-"
---

# IRepSettingsExportPropertiesInt.RemoveAll

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: RemoveAll for Properties

Deletes all custom properties in DIAdem REPORT for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyExport = dd.Report.Settings.Export
oMyProperties = oMyExport.Properties
oMyProperties.RemoveAll()
oMyProperty = oMyProperties.Add("Company")
oMyProperty.DataType = dd.ePropertyDataTypeString
oMyProperty.Value = "NI"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_RemoveAll_IRepSettingsExportPropertiesInt.htm`*

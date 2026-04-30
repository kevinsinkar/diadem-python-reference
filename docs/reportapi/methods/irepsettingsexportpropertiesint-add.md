---
title: "IRepSettingsExportPropertiesInt.Add"
description: "Creates a custom property in DIAdem REPORT for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or "
---

# IRepSettingsExportPropertiesInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for Properties

Creates a custom property in DIAdem REPORT for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
return_value = obj.Add(Name, Value, DataType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePropertyDataTypeInt32` | 3 | 32-bit integer |
| `ePropertyDataTypeFloat64` | 10 | 64-bit real |
| `ePropertyDataTypeString` | 23 | Text |
| `ePropertyDataTypeDate` | 30 | Date/Time |

## Python example

```python
oMyProperty = dd.Report.Settings.Export.Properties.Add("Company","NI", dd.ePropertyDataTypeString)
dd.Report.Sheets.ExportToPDF(dd.ScriptWritePath + "MyFile.pdf",False)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepSettingsExportPropertiesInt.htm`*

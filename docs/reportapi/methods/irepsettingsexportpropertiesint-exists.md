---
title: "IRepSettingsExportPropertiesInt.Exists"
description: "Checks in DIAdem REPORT whether a custom property for the export of the layout already exists. If you export the layout as an Office file in XML format, or as a"
---

# IRepSettingsExportPropertiesInt.Exists

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Exists for Properties

Checks in DIAdem REPORT whether a custom property for the export of the layout already exists. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyExport = dd.Report.Settings.Export
oMyProperties = oMyExport.Properties
if not(oMyProperties.Exists("Company")) :
    oMyProperty = oMyProperties.Add("Company")
    oMyProperty.DataType = dd.ePropertyDataTypeString
    oMyProperty.Value = "NI"
dd.Report.Sheets.ExportToPDF(dd.ScriptWritePath + "MyFile.pdf",False)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Exists_IRepSettingsExportPropertiesInt.htm`*

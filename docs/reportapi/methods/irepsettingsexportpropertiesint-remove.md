---
title: "IRepSettingsExportPropertiesInt.Remove"
description: "Deletes a custom property in DIAdem REPORT for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or "
---

# IRepSettingsExportPropertiesInt.Remove

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Remove for Properties

Deletes a custom property in DIAdem REPORT for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
obj.Remove(Name)
```

## Python example

```python
oMyExport = dd.Report.Settings.Export
oMyProperties = oMyExport.Properties
if oMyProperties.Exists("Company") :
    oMyProperties.Remove("Company")
oMyProperty = dd.Report.Settings.Export.Properties.Add("Company","NI", dd.ePropertyDataTypeString)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Remove_IRepSettingsExportPropertiesInt.htm`*

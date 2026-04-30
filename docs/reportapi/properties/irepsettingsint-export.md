---
title: "IRepSettingsInt.Export"
description: "The Export object provides the export properties in DIAdem REPORT. DIAdem saves the export properties in the layout. The export properties contain the Propertie"
---

# IRepSettingsInt.Export

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Export for Settings

The Export object provides the export properties in DIAdem REPORT. DIAdem saves the export properties in the layout. The export properties contain the Properties collection with a list of user-defined custom properties of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
return_value = obj.Export
```

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

*Source: `ReportApi/properties/Report_property_Export_IRepSettingsInt.htm`*

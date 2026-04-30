---
title: "IRepSettingsExportInt"
description: "The Export object provides the export properties in DIAdem REPORT. DIAdem saves the export properties in the layout. The export properties contain the Propertie"
---

# IRepSettingsExportInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Export

The Export object provides the export properties in DIAdem REPORT. DIAdem saves the export properties in the layout. The export properties contain the Properties collection with a list of custom properties for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Python example

```python
oMyProperty = dd.Report.Settings.Export.Properties.Add("Company","NI", dd.ePropertyDataTypeString)
dd.Report.Sheets.ExportToPDF(dd.ScriptWritePath + "MyFile.pdf",False)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsexportint-properties/">Properties</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepsettingsint/">Settings</a>.<a href="../../properties/irepsettingsint-export/">Export</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsExportInt.htm`*

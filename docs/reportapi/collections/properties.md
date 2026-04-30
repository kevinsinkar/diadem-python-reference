---
title: "Properties"
description: "The Properties collection provides a list of custom properties for the export of the layout in DIAdem REPORT. If you export the layout as an Office file in XML "
---

# Properties

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: Properties

The Properties collection provides a list of custom properties for the export of the layout in DIAdem REPORT. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Python example

```python
oMyProperty = dd.Report.Settings.Export.Properties.Add("Company","NI", dd.ePropertyDataTypeString)
dd.Report.Sheets.ExportToPDF(dd.ScriptWritePath + "MyFile.pdf",False)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsexportpropertiesint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepsettingsexportpropertiesint-add/">Add</a> | <a href="../../methods/irepsettingsexportpropertiesint-exists/">Exists</a> | <a href="../../methods/irepsettingsexportpropertiesint-item/">Item</a> | <a href="../../methods/irepsettingsexportpropertiesint-remove/">Remove</a> | <a href="../../methods/irepsettingsexportpropertiesint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepsettingsexportint/">Export</a>.<a href="../../properties/irepsettingsexportint-properties/">Properties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsExportPropertiesInt.htm`*

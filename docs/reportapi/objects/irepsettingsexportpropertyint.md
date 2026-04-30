---
title: "IRepSettingsExportPropertyInt"
description: "The Property object provides a custom property for the export of the layout in DIAdem REPORT. If you export the layout as an Office file in XML format, or as a "
---

# IRepSettingsExportPropertyInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Property

The Property object provides a custom property for the export of the layout in DIAdem REPORT. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Python example

```python
oMyProperty = dd.Report.Settings.Export.Properties.Add("Company","NI", dd.ePropertyDataTypeString)
dd.Report.Sheets.ExportToPDF(dd.ScriptWritePath + "MyFile.pdf",False)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsettingsexportpropertyint-datatype/">DataType</a> | <a href="../../properties/irepsettingsexportpropertyint-expressionvalue/">ExpressionValue</a> | <a href="../../properties/irepsettingsexportpropertyint-name/">Name</a> | <a href="../../properties/irepsettingsexportpropertyint-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/properties/">Properties</a>.<a href="../../methods/irepsettingsexportpropertiesint-add/">Add</a> | <a href="../../collections/properties/">Properties</a>.<a href="../../methods/irepsettingsexportpropertiesint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSettingsExportPropertyInt.htm`*

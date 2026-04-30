---
title: "IRepSettingsExportPropertyInt.Value"
description: "Specifies the value of a custom property for the export of the layout or of the master layout in DIAdem REPORT. The value can also be a DIAdem expression . If t"
---

# IRepSettingsExportPropertyInt.Value

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Value for Property

Specifies the value of a custom property for the export of the layout or of the master layout in DIAdem REPORT. The value can also be a DIAdem expression . If the property Value for Property does not contain a DIAdem expression, the properties ExpressionValue and Value are the same. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
obj.Value
```

## Python example

```python
oMyExport = dd.Report.Settings.Export
oMyProperties = oMyExport.Properties
sOutput = "Export Properties of Layout: " + oMyProperties.Count + "\r\n"
for oMyProperty in oMyProperties:
    sOutput = sOutPut + "Name: " + oMyProperty.Name + "\r\n"
    sOutput = sOutPut + "Value: " + oMyProperty.Value + "\r\n"
    sOutput = sOutPut + "Expression value: " + oMyProperty.ExpressionValue + "\r\n"
oMyMasterProperties = oMyExport.MasterLayoutProperties
sOutput = sOutput + "\r\n" + "Export Properties of Masterlayoiut: " + oMyMasterProperties.Count + "\r\n"
for oMyMasterProperty in oMyMasterProperties:
    sOutput = sOutPut + "Name: " + oMyMasterProperty.Name + "\r\n"
    sOutput = sOutPut + "Value: " + oMyMasterProperty.Value + "\r\n"
    sOutput = sOutPut + "Expression value: " + oMyMasterProperty.ExpressionValue + "\r\n"
print(sOutPut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Value_IRepSettingsExportPropertyInt.htm`*

---
title: "IRepSettingsExportInt.Properties"
description: "Returns in DIAdem REPORT all custom properties for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG-"
---

# IRepSettingsExportInt.Properties

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Properties for Export

Returns in DIAdem REPORT all custom properties for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
return_value = obj.Properties
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
<div class="SeeAlso"><h2> </h2>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Properties_IRepSettingsExportInt.htm`*

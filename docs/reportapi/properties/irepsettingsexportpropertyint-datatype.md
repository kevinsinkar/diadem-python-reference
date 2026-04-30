---
title: "IRepSettingsExportPropertyInt.DataType"
description: "Specifies the data type of a custom property for the export of the layout or of the master layout in DIAdem REPORT. If you export the layout as an Office file i"
---

# IRepSettingsExportPropertyInt.DataType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DataType for Property

Specifies the data type of a custom property for the export of the layout or of the master layout in DIAdem REPORT. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents. The type for the property names name , title , description , and author must be String , and the type for the property name datetime must be time . If you assign the incorrect type to a property name, an error occurs when you export the documents.

## Signature

```python
obj.DataType
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
oMyExport = dd.Report.Settings.Export
oMyProperties = oMyExport.Properties
sOutput = "Export Properties of Layout: " + oMyProperties.Count + "\r\n"
for oMyProperty in oMyProperties:
    sOutput = sOutPut + "Name: " + oMyProperty.Name + "\r\n"
    sOutput = sOutPut + "Value: " + oMyProperty.Value + "\r\n"
    sOutput = sOutPut + "Expression value: " + oMyProperty.ExpressionValue + "\r\n"
    sOutput = sOutPut + "Date type: " + oMyProperty.DataType + "\r\n"
oMyMasterProperties = oMyExport.MasterLayoutProperties
sOutput = sOutput + "\r\n" + "Export Properties of Masterlayoiut: " + oMyMasterProperties.Count + "\r\n"
for oMyMasterProperty in oMyMasterProperties:
    sOutput = sOutPut + "Name: " + oMyMasterProperty.Name + "\r\n"
    sOutput = sOutPut + "Value: " + oMyMasterProperty.Value + "\r\n"
    sOutput = sOutPut + "Expression value: " + oMyMasterProperty.ExpressionValue + "\r\n"
    sOutput = sOutPut + "Date type: " + oMyMasterProperty.DataType + "\r\n"
print(sOutPut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DataType_IRepSettingsExportPropertyInt.htm`*

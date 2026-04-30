---
title: "IRepSettingsExportPropertyInt.Name"
description: "Specifies the name of a custom property for the export of the layout or of the master layout in DIAdem REPORT. If you use the same name in the layout and in the"
---

# IRepSettingsExportPropertyInt.Name

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Name for Property

Specifies the name of a custom property for the export of the layout or of the master layout in DIAdem REPORT. If you use the same name in the layout and in the associated master layout and you export the layout as an Office file in XML-Format, or as a PDF-, JPEG-, PNG- or TIFF- file, DIAdem saves the properties of the layout as meta properties in the document instead of the properties of the master layout. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
obj.Name
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

*Source: `ReportApi/properties/Report_property_Name_IRepSettingsExportPropertyInt.htm`*

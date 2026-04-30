---
title: "IRepSettingsExportPropertiesInt.Item"
description: "Returns in DIAdem REPORT the custom property associated with a specific name or index for the export of the layout. If you export the layout as an Office file i"
---

# IRepSettingsExportPropertiesInt.Item

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Item for Properties

Returns in DIAdem REPORT the custom property associated with a specific name or index for the export of the layout. If you export the layout as an Office file in XML format, or as a PDF-, JPEG-, PNG- or TIFF-file, DIAdem saves these properties as meta properties in the document. Use Document <Data> to access the meta properties in exported documents.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyExport = dd.Report.Settings.Export
oMyProperties = oMyExport.Properties
sOutput = "Export Properties of Layout: " + oMyProperties.Count + "\r\n"
for I in range( 1, oMyProperties.Count+1):
    sOutput = sOutPut + "Name: " + oMyProperties(i).Name + "\r\n"
    sOutput = sOutPut + "Value: " + oMyProperties(i).Value + "\r\n"
    sOutput = sOutPut + "Expression value: " + oMyProperties(i).ExpressionValue + "\r\n"
oMyMasterProperties = oMyExport.MasterLayoutProperties
sOutput = sOutput + "\r\n" + "Export Properties of Masterlayoiut: " + oMyMasterProperties.Count + "\r\n"
for I in range( 1, oMyMasterProperties.Count+1):
    sOutput = sOutPut + "Name: " + oMyMasterProperties(I).Name + "\r\n"
    sOutput = sOutPut + "Value: " + oMyMasterProperties(I).Value + "\r\n"
    sOutput = sOutPut + "Expression value: " + oMyMasterProperties(I).ExpressionValue + "\r\n"
print(sOutPut)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Item_IRepSettingsExportPropertiesInt.htm`*

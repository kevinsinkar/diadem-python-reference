---
title: "ICSVExportParameter.StringSign"
description: "Specifies the characters that enclose text in the exported file when data is exported with the CSV_Export DataPlugin. You can use any character, but you can spe"
---

# ICSVExportParameter.StringSign

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: StringSign for CSVExportParameter <Navigator>

Specifies the characters that enclose text in the exported file when data is exported with the CSV_Export DataPlugin. You can use any character, but you can specify only one character.

## Signature

```python
obj.StringSign
```

## Python example

```python
oMyExportParameter = dd.Navigator.Settings.CreateDataPluginParameter("CSV_Export")
if IsObject(oMyExportParameter) :
    oMyExportParameter.DecimalSign = dd.eCSVExportDecimalSignPoint
    oMyExportParameter.Delimiter = dd.eCSVExportDelimiterSemicolon
    oMyExportParameter.Encoding = dd.eCSVExportEncodingAnsi
    oMyExportParameter.StringSign = "'"
    oMyExportParameter.TimeFormat = "#dd/mm/yyyy hh:nn:ss.ffff"
    dd.DataFileSave("D:\\MyNewData.csv", oMyExportParameter)
else:
    print("Parametrization not possible")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_StringSign_ICSVExportParameter.htm`*

---
title: "ICSVExportParameter.Delimiter"
description: "Specifies which character DIAdem uses as separator for the data of the exported file, when data is exported with the CSV_Export DataPlugin. The delimiter charac"
---

# ICSVExportParameter.Delimiter

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Delimiter for CSVExportParameter <Navigator>

Specifies which character DIAdem uses as separator for the data of the exported file, when data is exported with the CSV_Export DataPlugin. The delimiter character must be different to the decimal sign.

## Signature

```python
obj.Delimiter
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCSVExportDelimiterTab` | 0 | Tabulator |
| `eCSVExportDelimiterComma` | 1 | Comma |
| `eCSVExportDelimiterSemicolon` | 2 | Semicolon |
| `eCSVExportDelimiterSpace` | 3 | Blank |

## Python example

```python
MyPluginName = "CSV_Export"
oMyExportParameter = dd.Navigator.Settings.CreateDataPluginParameter(MyPluginName)
if IsObject(oMyExportParameter) :
    oMyExportParameter.DecimalSign = dd.eCSVExportDecimalSignPoint
    oMyExportParameter.Delimiter = dd.eCSVExportDelimiterSemicolon
    oMyExportParameter.Encoding = dd.eCSVExportEncodingAnsi
    oMyExportParameter.StringSign = "'"
    oMyExportParameter.TimeFormat = "#dd/mm/yyyy hh:nn:ss.ffff"
    dd.DataFileSave("D:\\MyNewData.csv", oMyExportParameter)
else:
    dd.DataFileSave("D:\\MyNewData.csv", MyPluginName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Delimiter_ICSVExportParameter.htm`*

---
title: "ICSVExportParameter.DecimalSign"
description: "Specifies which decimal symbol DIAdem uses for the exported file, when data is exported with the CSV_Export DataPlugin. The decimal sign must be different to th"
---

# ICSVExportParameter.DecimalSign

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DecimalSign for CSVExportParameter <Navigator>

Specifies which decimal symbol DIAdem uses for the exported file, when data is exported with the CSV_Export DataPlugin. The decimal sign must be different to the delimiter character.

## Signature

```python
obj.DecimalSign
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCSVExportDecimalSignPoint` | 0 | Point |
| `eCSVExportDecimalSignComma` | 1 | Comma |

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

*Source: `ScriptNavi/properties/navigator_property_DecimalSign_ICSVExportParameter.htm`*

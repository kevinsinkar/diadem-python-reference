---
title: "ICSVExportParameter.Encoding"
description: "Specifies which coding DIAdem uses for the data of the exported file, when data is exported with the CSV_Export DataPlugin."
---

# ICSVExportParameter.Encoding

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Encoding for CSVExportParameter <Navigator>

Specifies which coding DIAdem uses for the data of the exported file, when data is exported with the CSV_Export DataPlugin.

## Signature

```python
obj.Encoding
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCSVExportEncodingUnicode` | 0 | Unicode |
| `eCSVExportEncodingAnsi` | 1 | ANSI |

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

*Source: `ScriptNavi/properties/navigator_property_Encoding_ICSVExportParameter.htm`*

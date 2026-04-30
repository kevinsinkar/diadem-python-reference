---
title: "ICSVExportParameter.TimeFormat"
description: "Specifies which Date/time format DIAdem uses for the data of the exported file, when data is exported with the CSV_Export DataPlugin. You can use all Date/time "
---

# ICSVExportParameter.TimeFormat

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: TimeFormat for CSVExportParameter <Navigator>

Specifies which Date/time format DIAdem uses for the data of the exported file, when data is exported with the CSV_Export DataPlugin. You can use all Date/time formats available in DIAdem.

## Signature

```python
obj.TimeFormat
```

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

*Source: `ScriptNavi/properties/navigator_property_TimeFormat_ICSVExportParameter.htm`*

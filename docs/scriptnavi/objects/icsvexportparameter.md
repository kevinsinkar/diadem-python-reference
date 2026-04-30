---
title: "ICSVExportParameter"
description: "The CSVExportParameter <Navigator> object provides the properties and methods for parameterizing the export of data with the CSV_Export DataPlugin."
---

# ICSVExportParameter

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: CSVExportParameter <Navigator>

The CSVExportParameter <Navigator> object provides the properties and methods for parameterizing the export of data with the CSV_Export DataPlugin.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icsvexportparameter-datapluginname/">DataPluginName</a> | <a href="../../properties/icsvexportparameter-decimalsign/">DecimalSign</a> | <a href="../../properties/icsvexportparameter-delimiter/">Delimiter</a> | <a href="../../properties/icsvexportparameter-encoding/">Encoding</a> | <a href="../../properties/icsvexportparameter-stringsign/">StringSign</a> | <a href="../../properties/icsvexportparameter-timeformat/">TimeFormat</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icsvexportparameter-showdialog/">ShowDialog</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../inavigatorsettings/">Settings &lt;Navigator&gt;</a>.<a href="../../methods/inavigatorsettings-createdatapluginparameter/">CreateDataPluginParameter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ICSVExportParameter.htm`*

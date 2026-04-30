---
title: "INavigatorSettings.CreateDataPluginParameter"
description: "Creates an object with properties you use to configure a DataPlugin. For example, you can change the default DataPlugin configuration by configuring the \"CSV_Ex"
---

# INavigatorSettings.CreateDataPluginParameter

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateDataPluginParameter for Settings <Navigator>

Creates an object with properties you use to configure a DataPlugin. For example, you can change the default DataPlugin configuration by configuring the "CSV_Export" DataPlugin to create a target file with different file coding, different delimiters, or different decimal symbols. A description of the properties and methods for the DataPlugin named "CSV_Export" can be found on the page of the CSVExportParameter <Navigator> object. Note If the CreateDataPluginParameter method does not return an object, you cannot configure the selected DataPlugin.

## Signature

```python
return_value = obj.CreateDataPluginParameter(DataPluginName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If the <span class="Monospace">CreateDataPluginParameter</span> method does not return an object, you cannot configure the selected DataPlugin.</td></tr></table>
</div>

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

*Source: `ScriptNavi/methods/navigator_method_CreateDataPluginParameter_INavigatorSettings.htm`*

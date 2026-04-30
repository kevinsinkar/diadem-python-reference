---
title: "IDataPluginParameter.ShowDialog"
description: "Opens the dialog box where you configure the parameters of the selected DataPlugin."
---

# IDataPluginParameter.ShowDialog

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: ShowDialog for DataPluginParameter <Navigator>

Opens the dialog box where you configure the parameters of the selected DataPlugin.

## Signature

```python
sShowDialog = Object.ShowDialog()
```

## Python example

```python
oMyDPParams = dd.Navigator.Settings.CreateDataPluginParameter("CSV_Export")
oMyDPParams.DecimalSign = dd.eCSVExportDecimalSignComma
oMyDPParams.TimeFormat = "#dd/mm/yyyy hh:nn:ss.ffff"
if oMyDPParams.ShowDialog == "IDOk" :
    dd.DataFileSave("D:\\dd.Data.csv", oMyDPParams)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_ShowDialog_IDataPluginParameter.htm`*

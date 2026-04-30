---
title: "ICommonExportParameter.ShowDialog"
description: "Opens the dialog box where you configure the export of data with a specified DataPlugin."
---

# ICommonExportParameter.ShowDialog

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: ShowDialog for CommonExportParameter <Navigator>

Opens the dialog box where you configure the export of data with a specified DataPlugin.

## Signature

```python
sShowDialog = Object.ShowDialog()
```

## Python example

```python
oMyDataPluginExport = dd.Navigator.Settings.CreateDataPluginParameter("CSV_Export")
if IsObject(oMyDataPluginExport) :
    print(oMyDataPluginExport.DataPluginName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_ShowDialog_ICommonExportParameter.htm`*

---
title: "ICommonExportParameter.DataPluginName"
description: "Specifies the name of the DataPlugin when configuring the export of data with a selected DataPlugin."
---

# ICommonExportParameter.DataPluginName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DataPluginName for CommonExportParameter <Navigator>

Specifies the name of the DataPlugin when configuring the export of data with a selected DataPlugin.

## Signature

```python
obj.DataPluginName
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

*Source: `ScriptNavi/properties/navigator_property_DataPluginName_ICommonExportParameter.htm`*

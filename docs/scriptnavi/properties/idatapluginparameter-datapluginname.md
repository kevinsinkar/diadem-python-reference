---
title: "IDataPluginParameter.DataPluginName"
description: "During the configuration of a DataPlugin, specifies the name of the DataPlugin for which the object was created."
---

# IDataPluginParameter.DataPluginName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DataPluginName for DataPluginParameter <Navigator>

During the configuration of a DataPlugin, specifies the name of the DataPlugin for which the object was created.

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

*Source: `ScriptNavi/properties/navigator_property_DataPluginName_IDataPluginParameter.htm`*

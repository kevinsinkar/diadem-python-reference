---
title: "INavigatorSettings.LoadBrowseSettings"
description: "Loads Browse Settings . Browse settings have the filename extension *.tbs ."
---

# INavigatorSettings.LoadBrowseSettings

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadBrowseSettings for Settings <Navigator>

Loads Browse Settings . Browse settings have the filename extension *.tbs .

## Signature

```python
return_value = obj.LoadBrowseSettings(FileNamePath, DataStore)
```

## Python example

```python
oMyStore = dd.Navigator.Display.CurrDataStore.GetDataStore()
dd.Navigator.Settings.LoadBrowseSettings("D:\\MyBrowseSettings.tbs", oMyStore)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadBrowseSettings_INavigatorSettings.htm`*

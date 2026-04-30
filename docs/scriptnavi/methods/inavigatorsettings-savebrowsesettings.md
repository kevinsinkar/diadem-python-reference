---
title: "INavigatorSettings.SaveBrowseSettings"
description: "Saves all the given Browse Settings in a file with the extension *.tbs ."
---

# INavigatorSettings.SaveBrowseSettings

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SaveBrowseSettings for Settings <Navigator>

Saves all the given Browse Settings in a file with the extension *.tbs .

## Signature

```python
obj.SaveBrowseSettings(FileNamePath, BrowseSettings)
```

## Python example

```python
oMyStore = dd.Navigator.Display.CurrDataStore.GetDataStore()
oMyBrowseSettings = dd.Navigator.Settings.LoadBrowseSettings("D:\\MyBrowseSettings.tbs", oMyStore)
dd.Navigator.Settings.SaveBrowseSettings("D:\\MyNewBrowseSettings.tbs", oMyBrowseSettings)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SaveBrowseSettings_INavigatorSettings.htm`*

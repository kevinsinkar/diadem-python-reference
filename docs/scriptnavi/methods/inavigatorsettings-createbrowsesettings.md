---
title: "INavigatorSettings.CreateBrowseSettings"
description: "Creates the standard browse settings for the given data store and assigns the browse settings to an object."
---

# INavigatorSettings.CreateBrowseSettings

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateBrowseSettings for Settings <Navigator>

Creates the standard browse settings for the given data store and assigns the browse settings to an object.

## Signature

```python
return_value = obj.CreateBrowseSettings(DataStore)
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyBrowseSettings = dd.navigator.Settings.CreateBrowseSettings(oMyDataStore)
dd.Navigator.Settings.SaveBrowseSettings("D:\\MyNewBrowseSettings.tbs", oMyBrowseSettings)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_CreateBrowseSettings_INavigatorSettings.htm`*

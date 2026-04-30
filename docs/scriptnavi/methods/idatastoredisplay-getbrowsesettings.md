---
title: "IDataStoreDisplay.GetBrowseSettings"
description: "Determines the Browse Settings of a data store open in DIadem NAVIGATOR."
---

# IDataStoreDisplay.GetBrowseSettings

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetBrowseSettings for DataStoreDisplay

Determines the Browse Settings of a data store open in DIadem NAVIGATOR.

## Signature

```python
return_value = obj.GetBrowseSettings()
```

## Python example

```python
oMyBrowseSettings = dd.Navigator.Display.CurrDataStore.GetBrowseSettings()
dd.MsgBoxDisp(oMyBrowseSettings.RootEntity.EntityType.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetBrowseSettings_IDataStoreDisplay.htm`*

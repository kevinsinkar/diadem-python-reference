---
title: "ITDMDataStore.GetBrowseSettings"
description: "Determines the Browse settings of a data store."
---

# ITDMDataStore.GetBrowseSettings

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetBrowseSettings for DataStore

Determines the Browse settings of a data store.

## Signature

```python
return_value = obj.GetBrowseSettings()
```

## Python example

```python
oMyBrowseSettings = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example").GetBrowseSettings()
dd.MsgBoxDisp(oMyBrowseSettings.RootEntity.EntityType.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetBrowseSettings_ITDMDataStore.htm`*

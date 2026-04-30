---
title: "IUpdateSource.UpdateAll"
description: "Updates all DataPlugins registered on your computer according to the update source. If a DataPlugin is no longer up-to-date, the UpdateAll method overwrites the"
---

# IUpdateSource.UpdateAll

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: UpdateAll for UpdateSource <Navigator>

Updates all DataPlugins registered on your computer according to the update source. If a DataPlugin is no longer up-to-date, the UpdateAll method overwrites the local version with the current version.

## Signature

```python
bUpdateAll = Object.UpdateAll()
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyDataUpdateSource.UpdateAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_UpdateAll_IUpdateSource.htm`*

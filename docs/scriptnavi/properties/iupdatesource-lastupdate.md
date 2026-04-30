---
title: "IUpdateSource.LastUpdate"
description: "Specifies when the information about DataPlugins available in the update source was updated last."
---

# IUpdateSource.LastUpdate

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: LastUpdate for UpdateSource <Navigator>

Specifies when the information about DataPlugins available in the update source was updated last.

## Signature

```python
obj.LastUpdate
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
dd.MsgBoxDisp("Last update: " + oMyDataUpdateSource.LastUpdate + "\r\n" + "Number of DataPlugins to be updated: " + oMyDataUpdateSource.UpdateData.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_LastUpdate_IUpdateSource.htm`*

---
title: "IUpdateData.Count"
description: "Specifies the number of DataPlugins available in the update source."
---

# IUpdateData.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for UpdateData <Navigator>

Specifies the number of DataPlugins available in the update source.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_IUpdateData.htm`*

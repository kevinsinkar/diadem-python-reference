---
title: "IUpdateDataDataPlugin.Name"
description: "Specifies the name of a DataPlugin available in the update source."
---

# IUpdateDataDataPlugin.Name

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Name for UpdateDataDataPlugin <Navigator>

Specifies the name of a DataPlugin available in the update source.

## Signature

```python
obj.Name
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Name_IUpdateDataDataPlugin.htm`*

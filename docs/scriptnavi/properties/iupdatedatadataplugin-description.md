---
title: "IUpdateDataDataPlugin.Description"
description: "Specifies the description of DataPlugins available in the update source."
---

# IUpdateDataDataPlugin.Description

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Description for UpdateDataDataPlugin <Navigator>

Specifies the description of DataPlugins available in the update source.

## Signature

```python
obj.Description
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item("AOP").Description)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Description_IUpdateDataDataPlugin.htm`*

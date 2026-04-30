---
title: "IUpdateDataDataPlugin.Version"
description: "Specifies the version number of a DataPlugin in the update source."
---

# IUpdateDataDataPlugin.Version

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Version for UpdateDataDataPlugin <Navigator>

Specifies the version number of a DataPlugin in the update source.

## Signature

```python
obj.Version
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item("ADO").Version)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Version_IUpdateDataDataPlugin.htm`*

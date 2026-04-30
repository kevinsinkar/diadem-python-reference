---
title: "IUpdateDataDataPlugin.URL"
description: "Specifies the URL of a DataPlugin in the update source."
---

# IUpdateDataDataPlugin.URL

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: URL for UpdateDataDataPlugin <Navigator>

Specifies the URL of a DataPlugin in the update source.

## Signature

```python
obj.URL
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item("ADO").URL)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_URL_IUpdateDataDataPlugin.htm`*

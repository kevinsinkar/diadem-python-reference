---
title: "IRegisteredDataPlugin.IsSavingSupported"
description: "Specifies whether a DataPlugin supports saving data in a file."
---

# IRegisteredDataPlugin.IsSavingSupported

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsSavingSupported for RegisteredDataPlugin <Navigator>

Specifies whether a DataPlugin supports saving data in a file.

## Signature

```python
obj.IsSavingSupported
```

## Python example

```python
oMyRegisteredDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
dd.MsgBoxDisp(oMyRegisteredDataPlugins("Audio").IsSavingSupported )
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsSavingSupported_IRegisteredDataPlugin.htm`*

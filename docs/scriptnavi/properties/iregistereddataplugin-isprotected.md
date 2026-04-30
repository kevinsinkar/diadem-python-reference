---
title: "IRegisteredDataPlugin.IsProtected"
description: "Specifies whether a DataPlugin registered on your computer is protected. You cannot change or delete protected DataPlugins."
---

# IRegisteredDataPlugin.IsProtected

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsProtected for RegisteredDataPlugin <Navigator>

Specifies whether a DataPlugin registered on your computer is protected. You cannot change or delete protected DataPlugins.

## Signature

```python
obj.IsProtected
```

## Python example

```python
oMyRegisteredDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
dd.MsgBoxDisp(oMyRegisteredDataPlugins("Audio").IsProtected)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsProtected_IRegisteredDataPlugin.htm`*

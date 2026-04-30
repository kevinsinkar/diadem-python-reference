---
title: "IRegisteredDataPlugin.IsQuerySupported"
description: "Specifies whether a DataPlugin can process queries."
---

# IRegisteredDataPlugin.IsQuerySupported

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsQuerySupported for RegisteredDataPlugin <Navigator>

Specifies whether a DataPlugin can process queries.

## Signature

```python
obj.IsQuerySupported
```

## Python example

```python
oMyRegisteredDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
dd.MsgBoxDisp(oMyRegisteredDataPlugins("Audio").IsQuerySupported )
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsQuerySupported_IRegisteredDataPlugin.htm`*

---
title: "IRegisteredDataPluginCollection.Exists"
description: "Checks whether a DataPlugin with a specific name is already registered on your computer."
---

# IRegisteredDataPluginCollection.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for RegisteredDataPlugins <Navigator>

Checks whether a DataPlugin with a specific name is already registered on your computer.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
dd.MsgBoxDisp(dd.Navigator.Settings.RegisteredDataPlugins.Exists("CSV"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_IRegisteredDataPluginCollection.htm`*

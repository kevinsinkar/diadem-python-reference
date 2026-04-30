---
title: "IRegisteredDataPlugin.Name"
description: "Specifies the name of a DataPlugin registered on your computer."
---

# IRegisteredDataPlugin.Name

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Name for RegisteredDataPlugin <Navigator>

Specifies the name of a DataPlugin registered on your computer.

## Signature

```python
obj.Name
```

## Python example

```python
oMyDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
for DataPlugin in oMyDataPlugins:
    sOutput = sOutput + DataPlugin.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Name_IRegisteredDataPlugin.htm`*

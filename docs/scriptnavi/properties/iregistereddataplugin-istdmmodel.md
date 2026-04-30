---
title: "IRegisteredDataPlugin.IsTdmModel"
description: "Specifies whether a DataPlugin registered on your computer is based on the TDM data model and therefore provides TDM data."
---

# IRegisteredDataPlugin.IsTdmModel

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsTdmModel for RegisteredDataPlugin <Navigator>

Specifies whether a DataPlugin registered on your computer is based on the TDM data model and therefore provides TDM data.

## Signature

```python
obj.IsTdmModel
```

## Python example

```python
oMyDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
for DataPlugin in oMyDataPlugins:
    sOutput = sOutput + DataPlugin.Name + ": " + DataPlugin.IsTdmModel + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsTdmModel_IRegisteredDataPlugin.htm`*

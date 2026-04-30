---
title: "IRegisteredDataPlugin.IsFileBased"
description: "Specifies whether you can use a DataPlugin registered on your computer to load files."
---

# IRegisteredDataPlugin.IsFileBased

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsFileBased for RegisteredDataPlugin <Navigator>

Specifies whether you can use a DataPlugin registered on your computer to load files.

## Signature

```python
obj.IsFileBased
```

## Python example

```python
oMyRegisteredDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
for n in range( 1, oMyRegisteredDataPlugins.Count+1):
    if oMyRegisteredDataPlugins(n).IsFileBased == True :
        sOutput = sOutput + oMyRegisteredDataPlugins(n).Name + ": " + oMyRegisteredDataPlugins(n).FileExtensionList + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsFileBased_IRegisteredDataPlugin.htm`*

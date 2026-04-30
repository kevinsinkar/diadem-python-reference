---
title: "IUpdateDataDataPlugin.FileExtensionList"
description: "Specifies the list with filename extensions of DataPlugins available in the update source. DIAdem loads files with these filename extensions with the respective"
---

# IUpdateDataDataPlugin.FileExtensionList

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: FileExtensionList for UpdateDataDataPlugin <Navigator>

Specifies the list with filename extensions of DataPlugins available in the update source. DIAdem loads files with these filename extensions with the respective DataPlugin.

## Signature

```python
obj.FileExtensionList
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

*Source: `ScriptNavi/properties/navigator_property_FileExtensionList_IUpdateDataDataPlugin.htm`*

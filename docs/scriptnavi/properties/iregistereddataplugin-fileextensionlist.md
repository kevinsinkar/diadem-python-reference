---
title: "IRegisteredDataPlugin.FileExtensionList"
description: "Specifies the list with the filename extensions of the files which you can load with a registered DataPlugin. You can specify the list of filename extensions on"
---

# IRegisteredDataPlugin.FileExtensionList

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: FileExtensionList for RegisteredDataPlugin <Navigator>

Specifies the list with the filename extensions of the files which you can load with a registered DataPlugin. You can specify the list of filename extensions only for file-based DataPlugins. Use the IsFileBased method to determine whether a DataPlugin is file-based.

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

*Source: `ScriptNavi/properties/navigator_property_FileExtensionList_IRegisteredDataPlugin.htm`*

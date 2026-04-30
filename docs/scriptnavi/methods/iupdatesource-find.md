---
title: "IUpdateSource.Find"
description: "Specifies with which DataPlugins in the update source you can load files with the specified filename extension into DIAdem."
---

# IUpdateSource.Find

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Find for UpdateSource <Navigator>

Specifies with which DataPlugins in the update source you can load files with the specified filename extension into DIAdem.

## Signature

```python
vFind = Object.Find(Extension)
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
vDataPluginList = oMyDataUpdateSource.Find("DAT")
sOutput = "List of DataPlugins to load DAT files: " + "\r\n"
if not (len(vDataPluginList) == 0) :
    for sDataPluginName in vDataPluginList:
        sOutput = sOutput + sDataPluginName + "\r\n"
    dd.MsgBoxDisp(sOutput)
else:
    dd.MsgBoxDisp("No DataPlugins found")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Find_IUpdateSource.htm`*

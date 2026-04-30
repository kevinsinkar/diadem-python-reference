---
title: "IUpdateData.Exists"
description: "Checks whether a DataPlugin with a specified name is in the update source."
---

# IUpdateData.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for UpdateData <Navigator>

Checks whether a DataPlugin with a specified name is in the update source.

## Signature

```python
bExists = Object.Exists(Name)
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
if oMyUpdateData.Exists("GPX") :
    oPluginData = oMyUpdateData("GPX")
    if ((oPluginData.Type == dd.ePluginCodeVbCrypt) or (oPluginData.Type == dd.ePluginCodeVbs)) :
        oMyDataUpdateSource.Install("GPX", True)
    else:
        dd.MsgBoxDisp("DataPlugin " + oPluginData.Name + " is no VBCrypt or VBS DataPlugin." + "\r\n" + "Please install the DataPlugin manually from the NI website.")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_IUpdateData.htm`*

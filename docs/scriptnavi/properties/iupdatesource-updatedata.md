---
title: "IUpdateSource.UpdateData"
description: "Specifies the DataPlugins available in the update source."
---

# IUpdateSource.UpdateData

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: UpdateData for UpdateSource <Navigator>

Specifies the DataPlugins available in the update source.

## Signature

```python
return_value = obj.UpdateData
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

*Source: `ScriptNavi/properties/navigator_property_UpdateData_IUpdateSource.htm`*

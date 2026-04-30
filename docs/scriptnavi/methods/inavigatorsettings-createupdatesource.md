---
title: "INavigatorSettings.CreateUpdateSource"
description: "Generates the UpdateSource object which provides information about the DataPlugins in an update source. The generated object provides update methods for the Dat"
---

# INavigatorSettings.CreateUpdateSource

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateUpdateSource for Settings <Navigator>

Generates the UpdateSource object which provides information about the DataPlugins in an update source. The generated object provides update methods for the DataPlugins registered locally and methods for searching for DataPlugins for specified filename extensions. An update source is either the NI DataPlugin website or a DateFinder instance.

## Signature

```python
return_value = obj.CreateUpdateSource([Type], [Parameter])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eUpdateSourceNiWeb` | 42001 | The NI DataPlugin website is the update source. |
| `eUpdateSourceNiDFSE` | 42002 | The specified DataFinder instance is the update source. |

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
dd.MsgBoxDisp("Last update: " + oMyDataUpdateSource.LastUpdate + "\r\n" + "Number of DataPlugins to be updated: " + oMyDataUpdateSource.UpdateData.Count)
```

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource(dd.eUpdateSourceNiDFSE, "TestRig@DataFinder_instance")
oMyUpdateData = oMyDataUpdateSource.UpdateData
if oMyUpdateData.Exists("GPX") :
    oPluginData = oMyUpdateData("GPX")
    if ((oPluginData.Type == dd.ePluginCodeVbCrypt) or (oPluginData.Type == dd.ePluginCodeVbs)) :
        oMyDataUpdateSource.Install("GPX")
    else:
        dd.MsgBoxDisp("DataPlugin " + oPluginData.Name + " is no VBCrypt or VBS DataPlugin." + "\r\n" + "Please install the DataPlugin manually.")
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_CreateUpdateSource_INavigatorSettings.htm`*

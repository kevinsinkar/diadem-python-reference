---
title: "IUpdateSource.Parameter"
description: "Specifies the name of the DataFinder instance which you use as the source to update your local Data Plugins."
---

# IUpdateSource.Parameter

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Parameter for UpdateSource <Navigator>

Specifies the name of the DataFinder instance which you use as the source to update your local Data Plugins.

## Signature

```python
obj.Parameter
```

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource(dd.eUpdateSourceNiDFSE, "TestRig@DataFinder_Server")
dd.MsgBoxDisp("DataFinder Instance Name: " + oMyDataUpdateSource.Parameter + "\r\n" + "Last Update: " + oMyDataUpdateSource.LastUpdate)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Parameter_IUpdateSource.htm`*

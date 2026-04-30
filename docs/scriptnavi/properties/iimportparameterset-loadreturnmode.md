---
title: "IImportParameterSet.LoadReturnMode"
description: "Specifies with which elements a load command fills the returned elements list."
---

# IImportParameterSet.LoadReturnMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: LoadReturnMode for ImportParameter <Navigator>

Specifies with which elements a load command fills the returned elements list.

## Signature

```python
obj.LoadReturnMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLoadReturnHighestLevelElements` | 24130 | The load command returns the top Element<Data> which was changed by the load process. This can be the root, a list of channel groups, or a list of channels. |
| `eLoadReturnElements` | 24131 | Default setting. The load command returns a list of channel groups or a list of channels, depending on the loaded data. If the loaded data are channel groups or submatrices, the load command returns a list of channel groups. If the loaded data are channels or LocalColumns, DIAdem returns a list of channels. |
| `eLoadReturnGroupElements` | 24132 | The load command returns a list of channel groups. |
| `eLoadReturnChannelElements` | 24133 | The load command returns a list of channels. |

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingOnFirstAccess
oMyImportParameter.LoadReturnMode = dd.eLoadReturnElements
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_LoadReturnMode_IImportParameterSet.htm`*

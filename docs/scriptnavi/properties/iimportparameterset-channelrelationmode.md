---
title: "IImportParameterSet.ChannelRelationMode"
description: "Specifies whether DIAdem retains the channel reference between the x-channels to the y-channels when importing data."
---

# IImportParameterSet.ChannelRelationMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ChannelRelationMode for ImportParameter <Navigator>

Specifies whether DIAdem retains the channel reference between the x-channels to the y-channels when importing data.

## Signature

```python
obj.ChannelRelationMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eChnRelationNone` | 1 | DIAdem does not retain the xy-reference. |
| `eChnRelationXY` | 2 | DIAdem retains the xy-channel reference. |

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Append")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingImmediately
oMyImportParameter.ChannelRelationMode = dd.eChnRelationNone
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ChannelRelationMode_IImportParameterSet.htm`*

---
title: "IImportParameterSet.AppendCheckGroupName"
description: "Specifies how DIAdem deals with group names when appending external data to the data in the Data Portal."
---

# IImportParameterSet.AppendCheckGroupName

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: AppendCheckGroupName for ImportParameter <Navigator>

Specifies how DIAdem deals with group names when appending external data to the data in the Data Portal.

## Signature

```python
obj.AppendCheckGroupName
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAppendCheckGroupNameEqual` | 24140 | Default setting. DIAdem checks the name of the channel groups when appending and loading. If the channel groups do not have the same name, DIAdem does not append the data. |
| `eAppendCheckGroupNameNone` | 24141 | DIAdem does not check the name of the channel groups when appending and loading. DIAdem appends the external data to the internal data based on the index. |
| `eAppendCheckGroupNameAutomatic` | 24142 | If the external and internal data only contain one channel group each, DIAdem appends the external data to the internal data ignoring the name of the channel groups. If the external and the internal data contains more than one channel group, DIAdem checks the names of the channel groups when appending and loading and only appends the data if the names of the channel groups are identical. DIAdem does not append the external data to the internal data. |

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Append")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_AppendCheckGroupName_IImportParameterSet.htm`*

---
title: "IImportParameterSet.BulkDataLoadingMode"
description: "Specifies the time when DIAdem loads the mass data of the files, whose metadata was previously loaded with a load command, into the Data Portal."
---

# IImportParameterSet.BulkDataLoadingMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: BulkDataLoadingMode for ImportParameter <Navigator>

Specifies the time when DIAdem loads the mass data of the files, whose metadata was previously loaded with a load command, into the Data Portal.

## Signature

```python
obj.BulkDataLoadingMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBulkDataLoadingImmediately` | 24120 | Always load bulk data |
| `eBulkDataLoadingOnFirstAccess` | 24121 | Load bulk data on first access |
| `eBulkDataLoadingOnWriteAccess` | 24122 | Load bulk data on modification of channel data (Default) |

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingOnFirstAccess
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_BulkDataLoadingMode_IImportParameterSet.htm`*

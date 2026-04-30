---
title: "IImportParameterSet.ImportMode"
description: "Specifies whether a load command loads, registers, appends or expands the data."
---

# IImportParameterSet.ImportMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ImportMode for ImportParameter <Navigator>

Specifies whether a load command loads, registers, appends or expands the data.

## Signature

```python
obj.ImportMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLoad` | 24201 | Load (default) |
| `eRegister` | 24202 | Register |
| `eAppend` | 24203 | Append |
| `eExpand` | 24204 | Expand |

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyImportParameter.AppendCheckGroupName = dd.eAppendCheckGroupNameAutomatic
oMyImportParameter.BulkDataLoadingMode = dd.eBulkDataLoadingOnFirstAccess
oMyImportParameter.PropertyHandling.AutoUpdateChnCharacteristics = True
oMyImportParameter.PropertyHandling.InheritanceMode = dd.ePropInheritanceCopyToChannelLevel
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ImportMode_IImportParameterSet.htm`*

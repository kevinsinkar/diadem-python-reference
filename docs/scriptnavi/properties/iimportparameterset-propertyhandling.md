---
title: "IImportParameterSet.PropertyHandling"
description: "Contains the configuration of properties when loading data in DIAdem."
---

# IImportParameterSet.PropertyHandling

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: PropertyHandling for ImportParameter <Navigator>

Contains the configuration of properties when loading data in DIAdem.

## Signature

```python
return_value = obj.PropertyHandling
```

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

*Source: `ScriptNavi/properties/navigator_property_PropertyHandling_IImportParameterSet.htm`*

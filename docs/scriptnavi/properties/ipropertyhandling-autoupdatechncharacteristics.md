---
title: "IPropertyHandling.AutoUpdateChnCharacteristics"
description: "Specifies whether or not DIAdem calculates the characteristic values, when loading data automatically according to specific criteria. Per default DIAdem does no"
---

# IPropertyHandling.AutoUpdateChnCharacteristics

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: AutoUpdateChnCharacteristics for PropertyHandling <Navigator>

Specifies whether or not DIAdem calculates the characteristic values, when loading data automatically according to specific criteria. Per default DIAdem does not automatically calculate the characteristic values. If the loaded data did not contain characteristic values and DIAdem does not calculate characteristic values, this data is then missing in the data set.

## Signature

```python
obj.AutoUpdateChnCharacteristics
```

## Python example

```python
oMyImportParameter = dd.Navigator.Settings.CreateImportParameter("Load")
oMyImportParameter.PropertyHandling.AutoUpdateChnCharacteristics = True
oMyImportParameter.PropertyHandling.InheritanceMode = dd.ePropInheritanceCopyToChannelLevel
oMyImportParameter.PropertyHandling.InheritanceSeparator = dd.ePropInheritanceSeparatorTilde
oMyImportParameter.PropertyHandling.NamingSchema = dd.ePropNamingSchemaPropertyName
dd.DataFileLoad("Example.tdm", "TDM", oMyImportParameter)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_AutoUpdateChnCharacteristics_IPropertyHandling.htm`*

---
title: "IPropertyHandling.InheritanceSeparator"
description: "Specifies whether DIAdem uses the underscore or the tilde as the separator for the inheritance of properties."
---

# IPropertyHandling.InheritanceSeparator

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: InheritanceSeparator for PropertyHandling <Navigator>

Specifies whether DIAdem uses the underscore or the tilde as the separator for the inheritance of properties.

## Signature

```python
obj.InheritanceSeparator
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePropInheritanceSeparatorUnderscore` | 24151 | Underscore as separator |
| `ePropInheritanceSeparatorTilde` | 24152 | Tilde as separator (Default) |

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

*Source: `ScriptNavi/properties/navigator_property_InheritanceSeparator_IPropertyHandling.htm`*

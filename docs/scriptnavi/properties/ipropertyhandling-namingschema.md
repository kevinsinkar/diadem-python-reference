---
title: "IPropertyHandling.NamingSchema"
description: "Specifies the name pattern of properties after the properties are loaded into the Data Portal. If you load data from a DataFinder or an ASAM data store into the"
---

# IPropertyHandling.NamingSchema

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: NamingSchema for PropertyHandling <Navigator>

Specifies the name pattern of properties after the properties are loaded into the Data Portal. If you load data from a DataFinder or an ASAM data store into the Data Portal, DIAdem names the properties in the Data Portal according to these rules.

## Signature

```python
obj.NamingSchema
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePropNamingSchemaTypeNamePropertyName` | 24020 | Type_Property (Default) |
| `ePropNamingSchemaPathPropertyName` | 24021 | Path_Property |
| `ePropNamingSchemaPropertyName` | 24022 | Property |

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

*Source: `ScriptNavi/properties/navigator_property_NamingSchema_IPropertyHandling.htm`*

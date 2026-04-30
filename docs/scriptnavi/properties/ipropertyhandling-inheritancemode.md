---
title: "IPropertyHandling.InheritanceMode"
description: "Specifies whether DIAdem also transfers the properties of elements from superordinate levels to the element in the Data Portal when loading data from a DataFind"
---

# IPropertyHandling.InheritanceMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: InheritanceMode for PropertyHandling <Navigator>

Specifies whether DIAdem also transfers the properties of elements from superordinate levels to the element in the Data Portal when loading data from a DataFinder or an ASAM data store.

## Signature

```python
obj.InheritanceMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePropInheritanceNone` | 24010 | No inheritance (Default) |
| `ePropInheritanceMoveToLoadedLevel` | 24011 | Move to loaded level |
| `ePropInheritanceCopyToChannelLevel` | 24012 | Copy to channel level |

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

*Source: `ScriptNavi/properties/navigator_property_InheritanceMode_IPropertyHandling.htm`*

---
title: "IPropertyImportSet.InheritanceSeparator"
description: "Specifies for the Loading Configuration of an ASAM data store the inheritance separators of the properties, which DIAdem uses when loading data from data stores"
---

# IPropertyImportSet.InheritanceSeparator

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: InheritanceSeparator for PropertyImportSet

Specifies for the Loading Configuration of an ASAM data store the inheritance separators of the properties, which DIAdem uses when loading data from data stores into the Data Portal.

## Signature

```python
obj.InheritanceSeparator
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eInheritanceSeparatorAutomatic` | 24150 | Automatic separator |
| `eInheritanceSeparatorUnderscore` | 24151 | Underscore separator |
| `eInheritanceSeparatorTilde` | 24152 | Tilde separator |

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyPropertyImportSet = dd.Navigator.Settings.CreatePropertyImportSet(oMyStore)
oMyPropertyImportSet.NamingSchema = dd.eNamingSchemaPropertyName
oMyPropertyImportSet.InheritanceMode = dd.eInheritanceNone
oMyPropertyImportSet.InheritanceSeparator = dd.eInheritanceSeparatorAutomatic
dd.Navigator.Settings.SavePropertyImportSet("D:\\MyPropImportSet.tdl", oMyPropertyImportSet)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_InheritanceSeparator_IPropertyImportSet.htm`*

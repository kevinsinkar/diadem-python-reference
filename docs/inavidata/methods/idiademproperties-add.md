---
title: "IDiademProperties.Add"
description: "Generates a new property with a value in the script interface for internal data. If the property already exists, DIAdem changes only the value of the property. "
---

# IDiademProperties.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for Properties <Data>

Generates a new property with a value in the script interface for internal data. If the property already exists, DIAdem changes only the value of the property. If the property does not exist, DIAdem generates a new custom property. The Add method returns a Property object.

## Signature

```python
return_value = obj.Add(Name, Value, [DataType])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table5"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The value of the property must have the appropriate data type.</td></tr></table>
<table class="Borderless" id="table6"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can use the Navigator-API to assign date/time values to a DIAdem date/time property as a <a href="../../../scriptnavi/properties/itdmtimedisp-variantdate/">VariantDate</a> object or as a <a href="../../../scriptnavi/objects/itdmtimedisp/">UsiTimeDisp</a> object.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Enumeration` | 24 | DataTypeEnum |

## Python example

```python
dd.Data.Root.ChannelGroups(1).Properties.Add("Tester", "B.Counter")
```

```python
oMyDateTime = dd.Navigator.Display.CurrDataFinder.Browser.FocusedElement.Properties("DateTime").Value
dd.Data.Root.Properties.Add("DateTime_VariantDate", oMyDateTime.VariantDate, dd.DataTypeDate)
print(dd.Data.Root.Properties("DateTime_VariantDate").Value)
dd.Data.Root.Properties.Add("DateTime_VariantDate", oMyDateTime, dd.DataTypeDate)
print(dd.Data.Root.Properties("DateTime_VariantDate").Value)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_IDiademProperties.HTM`*

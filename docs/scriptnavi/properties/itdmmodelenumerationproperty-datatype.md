---
title: "ITDMModelEnumerationProperty.DataType"
description: "Specifies in a data store the data type of an enumeration property of the data model."
---

# ITDMModelEnumerationProperty.DataType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: DataType for ModelEnumerationProperty

Specifies in a data store the data type of an enumeration property of the data model.

## Signature

```python
obj.DataType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eNoType` | 0 | Not defined |
| `eI8` | 1 | 8-bit integer values |
| `eI16` | 2 | 16-bit integer values |
| `eI32` | 3 | 32-bit integer values |
| `eI64` | 4 | 64-bit integer values |
| `eByte` | 5 | Byte values |
| `eU16` | 6 | Unsigned 16-bit integer values |
| `eU32` | 7 | Unsigned 32-bit integer values |
| `eU64` | 8 | Unsigned 64-bit integer values |
| `eR32` | 9 | 32-bit real values |
| `eR64` | 10 | 64-bit real values |
| `eString` | 23 | Text |
| `eEnum` | 24 | Enumeration |
| `eTime` | 30 | Time values |

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
oMyEntity = oMyDataStoreModel.Entities("MeaQuantity")
dd.MsgBoxDisp(oMyEntity.ModelProperties(1).DataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_DataType_ITDMModelEnumerationProperty.htm`*

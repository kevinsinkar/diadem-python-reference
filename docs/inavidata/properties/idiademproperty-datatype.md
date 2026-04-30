---
title: "IDiademProperty.DataType"
description: "Specifies in the script interface for internal data the data type of a property or of a custom property."
---

# IDiademProperty.DataType

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DataType for Property <Data>

Specifies in the script interface for internal data the data type of a property or of a custom property.

## Signature

```python
obj.DataType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `Enumeration` | 24 | DataTypeEnum |

## Python example

```python
# Function to convert data type from integer into text ===
def PropertyDataTypeAsText(eMyType):
    select_variable_0 = eMyType
    if (select_variable_0 == dd.DataTypeEnum) :
        PropertyDataTypeAsText = "Enumeration"
    elif (select_variable_0 == dd.DataTypeFloat64) :
        PropertyDataTypeAsText = "Float64"
    elif (select_variable_0 == dd.DataTypeFloat32) :
        PropertyDataTypeAsText = "Float32"
    elif (select_variable_0 == dd.DataTypeInt16) :
        PropertyDataTypeAsText = "Int16"
    elif (select_variable_0 == dd.DataTypeInt32) :
        PropertyDataTypeAsText = "Int32"
    elif (select_variable_0 == dd.DataTypeString) :
        PropertyDataTypeAsText = "String"
    elif (select_variable_0 == dd.DataTypeUInt8) :
        PropertyDataTypeAsText = "UInt8"
    elif (select_variable_0 == dd.DataTypeDate) :
        PropertyDataTypeAsText = "Date"
    elif (select_variable_0 == dd.DataTypeUnknown) :
        PropertyDataTypeAsText = "Unknown"
    return PropertyDataTypeAsText

oMyProp = dd.Data.Root.ActiveChannelGroup.Channels(1).Properties(1)
print("Property name: " , oMyProp.Name , "\r\n" , "Data type: " , PropertyDataTypeAsText(oMyProp.DataType))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DataType_IDiademProperty.HTM`*

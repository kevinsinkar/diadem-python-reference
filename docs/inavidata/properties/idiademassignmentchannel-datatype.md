---
title: "IDiademAssignmentChannel.DataType"
description: "Specifies the data type of an assignment channel in the script interface for internal data."
---

# IDiademAssignmentChannel.DataType

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DataType for AssignmentChannel <Data>

Specifies the data type of an assignment channel in the script interface for internal data.

## Signature

```python
obj.DataType
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
dd.MsgBoxDisp(ChannelDataTypeAsText(oMyChn.DataType))

#Function to convert data type from integer into text
def ChannelDataTypeAsText(eMyType):
    select_variable_0 = eMyType
    if (select_variable_0 == dd.DataTypeFloat64) :
        ChannelDatatypeAsText = "Float64"
    elif (select_variable_0 == dd.DataTypeString) :
        ChannelDatatypeAsText = "String"
    elif (select_variable_0 == dd.DataTypeDate) :
        ChannelDatatypeAsText = "Date"
    return ChannelDataTypeAsText
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DataType_IDiademAssignmentChannel.htm`*

---
title: "IDiademComplexChannel.DataType"
description: "Returns the data type of a complex channel in the script interface for internal data."
---

# IDiademComplexChannel.DataType

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DataType for ComplexChannel <Data>

Returns the data type of a complex channel in the script interface for internal data.

## Signature

```python
obj.DataType
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If the data type of a channel is changed by a function or by the <a href="#" data-unresolved="1">DisplayType</a> channel property, you must first request the data type before you use other type-dependent properties.</td></tr></table>
</div>

## Python example

```python
oMyChn = dd.Data.Root.ChannelGroups(1).Channels(1)
dd.MsgBoxDisp ("Channel name: " + oMyChn.Name + "\r\n" + "Data type: " + ChannelDataTypeAsText(oMyChn.DataType) )

# Function to convert data type from integer into text ===
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
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_DataType_IDiademComplexChannel.htm`*

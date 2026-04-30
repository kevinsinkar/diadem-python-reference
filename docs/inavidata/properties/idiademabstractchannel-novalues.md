---
title: "IDiademAbstractChannel.NoValues"
description: "Specifies whether a channel contains NoValues."
---

# IDiademAbstractChannel.NoValues

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: NoValues for BaseChannel <Data>

Specifies whether a channel contains NoValues.

## Signature

```python
obj.NoValues
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTriStateFalse` | 0 | No NoValues |
| `eTriStateUnknown` | 1 | Unknown |

## Python example

```python
def NoValuesKey2Txt(mode):
    select_variable_0 = mode
    if (select_variable_0 == dd.eTriStateTrue) :
        NoValuesKey2Txt = "eTriStateTrue"
    elif (select_variable_0 == dd.eTriStateFalse) :
        NoValuesKey2Txt = "eTriStateFalse"
    elif (select_variable_0 == dd.eTriStateUnknown) :
        NoValuesKey2Txt = "eTriStateUnknown"
    return NoValuesKey2Txt

oMyChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
dd.MsgBoxDisp (NoValuesKey2Txt(oMyChannel.NoValues)) # equivalent to oMyChannel.Properties("novaluekey").Value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_NoValues_IDiademAbstractChannel.htm`*

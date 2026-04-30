---
title: "IDiademChannels.AddImplicitChannel"
description: "Creates a new implicit channel in the script interface for internal data."
---

# IDiademChannels.AddImplicitChannel

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddImplicitChannel for Channels <Data>

Creates a new implicit channel in the script interface for internal data.

## Signature

```python
return_value = obj.AddImplicitChannel(Name, StartValue, Increment, Size, DataType, [DestIndex])
```

## Python example

```python
oMyGroup = dd.Data.Root.ChannelGroups
oMyChannel = oMyGroup.Add("MyChnGrp").Channels.AddImplicitChannel("MyImplChn", 1, 1, 100,dd.DataTypeFloat64)
```

```python
oMyGroups = dd.Data.Root.ChannelGroups
oMyGroup = oMyGroups.Add("MyChnGrp")
oMyChannel = oMyGroup.Channels.AddImplicitChannel("MyImplChn", DateSerial(2015, 3, 15), float(3600*24), 100, dd.DataTypeDate)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddImplicitChannel_IDiademChannels.htm`*

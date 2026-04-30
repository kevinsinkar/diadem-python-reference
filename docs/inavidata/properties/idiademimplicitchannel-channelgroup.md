---
title: "IDiademImplicitChannel.ChannelGroup"
description: "Specifies the channel group which contains the specified implicit channel in the script interface for internal data."
---

# IDiademImplicitChannel.ChannelGroup

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ChannelGroup for ImplicitChannel <Data>

Specifies the channel group which contains the specified implicit channel in the script interface for internal data.

## Signature

```python
return_value = obj.ChannelGroup
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Demo1.tdm")
dd.MsgBoxDisp(dd.Data.GetChannel("Noise").ChannelGroup.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ChannelGroup_IDiademImplicitChannel.htm`*

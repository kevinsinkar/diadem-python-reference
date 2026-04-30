---
title: "IDiademAbstractChannel.RemoveValues"
description: "Deletes the specified values from a channel. DIAdem moves up the subsequent values."
---

# IDiademAbstractChannel.RemoveValues

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: RemoveValues for BaseChannel <Data>

Deletes the specified values from a channel. DIAdem moves up the subsequent values.

## Signature

```python
obj.RemoveValues([Index], [Count])
```

## Python example

```python
oMyChannel = dd.Data.Root.ActiveChannelGroup.Channels(1)
oMyChannel.RemoveValues(3, 4)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_RemoveValues_IDiademAbstractChannel.htm`*

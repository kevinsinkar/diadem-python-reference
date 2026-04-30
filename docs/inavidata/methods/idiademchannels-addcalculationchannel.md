---
title: "IDiademChannels.AddCalculationChannel"
description: "Generates, in the script interface for internal data, a new calculation channel in the current channel group with a simple single-line formula."
---

# IDiademChannels.AddCalculationChannel

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddCalculationChannel for Channels <Data>

Generates, in the script interface for internal data, a new calculation channel in the current channel group with a simple single-line formula.

## Signature

```python
return_value = obj.AddCalculationChannel(Name, Formula, [DestUnit], [DestIndex])
```

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddCalculationChannel_IDiademChannels.htm`*

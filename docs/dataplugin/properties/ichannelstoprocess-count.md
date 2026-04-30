---
title: "IChannelsToProcess.Count"
description: "Returns the number of elements in a ChannelsToProcess collection."
---

# IChannelsToProcess.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for ChannelsToProcess

Returns the number of elements in a ChannelsToProcess collection.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, ProcessedChn.Channels.Count + 1):
    ProcessedChn.Properties.Add(ProcessedChn.Channels(i).Name,"Composite")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IChannelsToProcess.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

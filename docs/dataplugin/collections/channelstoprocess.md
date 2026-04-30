---
title: "ChannelsToProcess"
description: "Collection of all the channels that a Processed channel comprises. Use the ChannelsToProcess collection to delete channels or to add new channels."
---

# ChannelsToProcess

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: ChannelsToProcess

Collection of all the channels that a Processed channel comprises. Use the ChannelsToProcess collection to delete channels or to add new channels.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, ProcessedChn.Channels.Count + 1):
    ProcessedChn.Properties.Add(ProcessedChn.Channels(i).Name,"Composite")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ichannelstoprocess-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ichannelstoprocess-add/">Add</a> | <a href="../../methods/ichannelstoprocess-item/">Item</a> | <a href="../../methods/ichannelstoprocess-remove/">Remove</a> | <a href="../../methods/ichannelstoprocess-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IChannelsToProcess.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

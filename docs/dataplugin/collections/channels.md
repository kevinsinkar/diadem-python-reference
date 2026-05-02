---
title: "Channels"
description: "Collection of all channels . Use the Channels collection to delete channels or to add new channels."
---

# Channels

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: Channels <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Collection of all channels . Use the Channels collection to delete channels or to add new channels.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyGrp = Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.Add("MyChannelNum",eR64)
for i in range(1, 100 + 1):
    oMyChn.Values(i) = cdbl(i/100000)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ichannels-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ichannels-add/">Add</a> | <a href="../../methods/ichannels-adddirectaccesschannel/">AddDirectAccessChannel</a> | <a href="../../methods/ichannels-addimplicitchannel/">AddImplicitChannel</a> | <a href="../../methods/ichannels-addprocessedchannel/">AddProcessedChannel</a> | <a href="../../methods/ichannels-addstorechannel/">AddStoreChannel</a> | <a href="../../methods/ichannels-exists/">Exists</a> | <a href="../../methods/ichannels-item/">Item</a> | <a href="../../methods/ichannels-remove/">Remove</a> | <a href="../../methods/ichannels-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">Store Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

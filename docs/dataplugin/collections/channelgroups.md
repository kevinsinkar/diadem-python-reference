---
title: "ChannelGroups"
description: "Collection of all channel groups . Use the ChannelGroups collection to delete channel groups or to add new channel groups."
---

# ChannelGroups

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: ChannelGroups <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Collection of all channel groups . Use the ChannelGroups collection to delete channel groups or to add new channel groups.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.ChannelGroups.RemoveAll
Root.ChannelGroups.Add("MyChannelGroup")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ichannelgroups-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ichannelgroups-add/">Add</a> | <a href="../../methods/ichannelgroups-exists/">Exists</a> | <a href="../../methods/ichannelgroups-item/">Item</a> | <a href="../../methods/ichannelgroups-remove/">Remove</a> | <a href="../../methods/ichannelgroups-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">Store Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IChannelGroups.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

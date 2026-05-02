---
title: "IRoot"
description: "The Root object provides the list of all channel groups and all properties of the data set."
---

# IRoot

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Root <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The Root object provides the list of all channel groups and all properties of the data set.

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
<p><a href="../../properties/iroot-channelgroups/">ChannelGroups</a> | <a href="../../properties/iroot-name/">Name</a> | <a href="../../properties/iroot-properties/">Properties</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iroot-importstore/">ImportStore</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iroot-importstore/">ImportStore</a></p>
</div>
<h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IRoot.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

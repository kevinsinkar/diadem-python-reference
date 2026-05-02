---
title: "Properties"
description: "A collection of all properties for the Root object, for the ChannelGroup object, or for the Channel object. The properties include the base properties of the da"
---

# Properties

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: Properties <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

A collection of all properties for the Root object, for the ChannelGroup object, or for the Channel object. The properties include the base properties of the data model and user-defined custom properties. You can use the Properties collection to delete or to add properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("DateTime",CreateTime(2004,6,12,12,17,55,0,0,0))
Root.Properties.Add("Author","CK")
```

```python
oMyChn.Properties.Add("unit_string", "°C")
oMyChn.Properties.Add("wf_xname", "Time")
oMyChn.Properties.Add("wf_xunit_string", "h")
oMyChn.Properties.Add("wf_start_offset", 0)
oMyChn.Properties.Add("wf_increment", 1)
oChannelGroup.Channels.AddDirectAccessChannel(oChn)
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/iproperties-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iproperties-add/">Add</a> | <a href="../../methods/iproperties-addproperties/">AddProperties</a> | <a href="../../methods/iproperties-exists/">Exists</a> | <a href="../../methods/iproperties-item/">Item</a> | <a href="../../methods/iproperties-remove/">Remove</a> | <a href="../../methods/iproperties-removeall/">RemoveAll</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Store Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

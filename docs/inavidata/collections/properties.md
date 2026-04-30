---
title: "Properties"
description: "Collection of all the properties of a data element for the Root object, the ChannelGroup object, or the Channel object, in the script interface for internal dat"
---

# Properties

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: Properties <Data>

Collection of all the properties of a data element for the Root object, the ChannelGroup object, or the Channel object, in the script interface for internal data. The properties include the base properties of the data model and custom properties. You use the Properties collection to access properties, and to delete or to add properties.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Refer to <a href="#" data-unresolved="1">Properties in DIAdem - Overview</a> for information about properties of files, groups, and channels.</td></tr></table>
</div>

## Python example

```python
dd.Data.Root.Properties.Add("Description","test")
dd.Data.Root.Properties.Add("Author","user")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademproperties-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademproperties-add/">Add</a> | <a href="../../methods/idiademproperties-addproperties/">AddProperties</a> | <a href="../../methods/idiademproperties-exists/">Exists</a> | <a href="../../methods/idiademproperties-item/">Item</a> | <a href="../../methods/idiademproperties-remove/">Remove</a> | <a href="../../methods/idiademproperties-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idiademassignmentchannel/">AssignmentChannel &lt;Data&gt;</a>.<a href="../../properties/idiademassignmentchannel-properties/">Properties</a> | <a href="../../objects/idiademcalculationchannel/">CalculationChannel &lt;Data&gt;</a>.<a href="../../properties/idiademcalculationchannel-properties/">Properties</a> | <a href="../../objects/idiademchannel/">Channel &lt;Data&gt;</a>.<a href="../../properties/idiademchannel-properties/">Properties</a> | <a href="../../objects/idiademchannelgroup/">ChannelGroup &lt;Data&gt;</a>.<a href="../../properties/idiademchannelgroup-properties/">Properties</a> | <a href="../../objects/idiademimplicitchannel/">ImplicitChannel &lt;Data&gt;</a>.<a href="../../properties/idiademimplicitchannel-properties/">Properties</a> | <a href="../../objects/idiademroot/">Root &lt;Data&gt;</a>.<a href="../../properties/idiademroot-properties/">Properties</a> | <a href="../../objects/idiademvideochannel/">VideoChannel &lt;Data&gt;</a>.<a href="../../properties/idiademvideochannel-properties/">Properties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademProperties.HTM`*

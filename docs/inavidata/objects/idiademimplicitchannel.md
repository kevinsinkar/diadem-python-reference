---
title: "IDiademImplicitChannel"
description: "The ImplicitChannel object provides an implicit channel in the interface for internal data. An implicit channel contains linear generation specifications, which"
---

# IDiademImplicitChannel

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: ImplicitChannel <Data>

The ImplicitChannel object provides an implicit channel in the interface for internal data. An implicit channel contains linear generation specifications, which describes the data, instead of single values.

## Python example

```python
oMyChn = dd.Data.Root.ChannelGroups(1).Channels.AddImplicitChannel("MyImplChn",1,5,100,dd.DataTypeFloat64)
dd.MsgBoxDisp ("Channel name: " + oMyChn.Name + "\r\n" + "Data type: " + oMyChn.DataType)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademimplicitchannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/idiademimplicitchannel-datatype/">DataType</a> | <a href="../../properties/idiademimplicitchannel-increment/">Increment</a> | <a href="../../properties/idiademimplicitchannel-isreadonly/">IsReadOnly</a> | <a href="../../properties/idiademimplicitchannel-maximum/">Maximum</a> | <a href="../../properties/idiademimplicitchannel-minimum/">Minimum</a> | <a href="../../properties/idiademimplicitchannel-name/">Name</a> | <a href="../../properties/idiademimplicitchannel-novalues/">NoValues</a> | <a href="../../properties/idiademimplicitchannel-operationalflags/">OperationalFlags</a> | <a href="../../properties/idiademimplicitchannel-properties/">Properties</a> | <a href="../../properties/idiademimplicitchannel-size/">Size</a> | <a href="../../properties/idiademimplicitchannel-startvalue/">StartValue</a> | <a href="../../properties/idiademimplicitchannel-unitsymbol/">UnitSymbol</a> | <a href="../../properties/idiademimplicitchannel-valueindex/">ValueIndex</a> | <a href="../../properties/idiademimplicitchannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademimplicitchannel-getreference/">GetReference</a> | <a href="../../methods/idiademimplicitchannel-getvaluesblock/">GetValuesBlock</a> | <a href="../../methods/idiademimplicitchannel-iskindof/">IsKindOf</a> | <a href="../../methods/idiademimplicitchannel-xrelation/">XRelation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addchannel/">AddChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addimplicitchannel/">AddImplicitChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-item/">Item</a> | <a href="../inavidata/">Data</a>.<a href="../../methods/inavidata-getchannel/">GetChannel</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademImplicitChannel.htm`*

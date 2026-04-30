---
title: "IDiademChannel"
description: "The Channel object provides a channel and the associated Properties in the script interface for internal data. The Channel object is an element of the Channels "
---

# IDiademChannel

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: Channel <Data>

The Channel object provides a channel and the associated Properties in the script interface for internal data. The Channel object is an element of the Channels collection.

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups.Add("MyChannelGroup")
oMyChn = oMyGrp.Channels.Add("MyChannel",dd.DataTypeFloat64)
for i in range( 1, 100+1):
    oMyChn = []
oMyChn.append(float(i/100000))
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademchannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/idiademchannel-datatype/">DataType</a> | <a href="../../properties/idiademchannel-isreadonly/">IsReadOnly</a> | <a href="../../properties/idiademchannel-maximum/">Maximum</a> | <a href="../../properties/idiademchannel-minimum/">Minimum</a> | <a href="../../properties/idiademchannel-name/">Name</a> | <a href="../../properties/idiademchannel-novalues/">NoValues</a> | <a href="../../properties/idiademchannel-operationalflags/">OperationalFlags</a> | <a href="../../properties/idiademchannel-properties/">Properties</a> | <a href="../../properties/idiademchannel-reservedsize/">ReservedSize</a> | <a href="../../properties/idiademchannel-size/">Size</a> | <a href="../../properties/idiademchannel-unitsymbol/">UnitSymbol</a> | <a href="../../properties/idiademchannel-valueindex/">ValueIndex</a> | <a href="../../properties/idiademchannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademchannel-getreference/">GetReference</a> | <a href="../../methods/idiademchannel-getvaluesblock/">GetValuesBlock</a> | <a href="../../methods/idiademchannel-iskindof/">IsKindOf</a> | <a href="../../methods/idiademchannel-removevalues/">RemoveValues</a> | <a href="../../methods/idiademchannel-setvalues/">SetValues</a> | <a href="../../methods/idiademchannel-setvaluesblock/">SetValuesBlock</a> | <a href="../../methods/idiademchannel-xrelation/">XRelation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idiademassignmentchannel/">AssignmentChannel &lt;Data&gt;</a>.<a href="../../methods/idiademassignmentchannel-xrelation/">XRelation</a> | <a href="../idiademcalculationchannel/">CalculationChannel &lt;Data&gt;</a>.<a href="../../methods/idiademcalculationchannel-xrelation/">XRelation</a> | <a href="./">Channel &lt;Data&gt;</a>.<a href="../../methods/idiademchannel-xrelation/">XRelation</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-add/">Add</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addchannel/">AddChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-item/">Item</a> | <a href="../idiademcomplexchannel/">ComplexChannel &lt;Data&gt;</a>.<a href="../../methods/idiademcomplexchannel-xrelation/">XRelation</a> | <a href="../inavidata/">Data</a>.<a href="../../methods/inavidata-getchannel/">GetChannel</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademimplicitchannel/">ImplicitChannel &lt;Data&gt;</a>.<a href="../../methods/idiademimplicitchannel-xrelation/">XRelation</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademChannel.HTM`*

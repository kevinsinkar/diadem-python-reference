---
title: "IDiademAbstractChannel"
description: "The BaseChannel object provides a channel and the associated Properties in the script interface for internal data. The BaseChannel object corresponds to one of "
---

# IDiademAbstractChannel

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: BaseChannel <Data>

The BaseChannel object provides a channel and the associated Properties in the script interface for internal data. The BaseChannel object corresponds to one of the following objects: AssignmentChannel (IDiademAssignmentChannel) Assignment channel CalculationChannel (IDiademCalculationChannel) Calculation Channel Channel (IDiademChannel) Numeric or text channel ImplicitChannel (IDiademImplicitChannel) Implicit channel

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
<p><a href="../../properties/idiademabstractchannel-datatype/">DataType</a> | <a href="../../properties/idiademabstractchannel-isreadonly/">IsReadOnly</a> | <a href="../../properties/idiademabstractchannel-maximum/">Maximum</a> | <a href="../../properties/idiademabstractchannel-minimum/">Minimum</a> | <a href="../../properties/idiademabstractchannel-name/">Name</a> | <a href="../../properties/idiademabstractchannel-novalues/">NoValues</a> | <a href="../../properties/idiademabstractchannel-properties/">Properties</a> | <a href="../../properties/idiademabstractchannel-unitsymbol/">UnitSymbol</a>| <a href="../../properties/idiademabstractchannel-valueindex/">ValueIndex</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademabstractchannel-getreference/">GetReference</a> | <a href="../../methods/idiademabstractchannel-getvaluesblock/">GetValuesBlock</a> | <a href="../../methods/idiademabstractchannel-iskindof/">IsKindOf</a> | <a href="../../methods/idiademabstractchannel-xrelation/">XRelation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addchannel/">AddChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-item/">Item</a> | <a href="../inavidata/">Data</a>.<a href="../../methods/inavidata-getchannel/">GetChannel</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademAbstractChannel.htm`*

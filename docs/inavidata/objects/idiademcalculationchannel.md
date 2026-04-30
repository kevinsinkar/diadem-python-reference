---
title: "IDiademCalculationChannel"
description: "The CalculationChannel <Data> object provides a calculation channel . Use the AddCalculationChannel method to create a new calculation channel using a simple si"
---

# IDiademCalculationChannel

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: CalculationChannel <Data>

The CalculationChannel <Data> object provides a calculation channel . Use the AddCalculationChannel method to create a new calculation channel using a simple single-line formula and the AddCalculationChannelRef method to create a new calculation channel with a reference to a calculation of the calculation manager.

## Python example

```python
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademcalculationchannel-calculationreference/">CalculationReference</a> | <a href="../../properties/idiademcalculationchannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/idiademcalculationchannel-datatype/">DataType</a> | <a href="../../properties/idiademcalculationchannel-destunit/">DestUnit</a> | <a href="../../properties/idiademcalculationchannel-formula/">Formula</a> | <a href="../../properties/idiademcalculationchannel-isreadonly/">IsReadOnly</a> | <a href="../../properties/idiademcalculationchannel-maximum/">Maximum</a> | <a href="../../properties/idiademcalculationchannel-minimum/">Minimum</a> | <a href="../../properties/idiademcalculationchannel-name/">Name</a> | <a href="../../properties/idiademcalculationchannel-novalues/">NoValues</a> | <a href="../../properties/idiademcalculationchannel-operationalflags/">OperationalFlags</a> | <a href="../../properties/idiademcalculationchannel-properties/">Properties</a> | <a href="../../properties/idiademcalculationchannel-quantitybased/">QuantityBased</a> | <a href="../../properties/idiademcalculationchannel-unitsymbol/">UnitSymbol</a> | <a href="../../properties/idiademcalculationchannel-valueindex/">ValueIndex</a> | <a href="../../properties/idiademcalculationchannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademcalculationchannel-getreference/">GetReference</a> | <a href="../../methods/idiademcalculationchannel-getvaluesblock/">GetValuesBlock</a> | <a href="../../methods/idiademcalculationchannel-iskindof/">IsKindOf</a> | <a href="../../methods/idiademcalculationchannel-runcalculation/">RunCalculation</a> | <a href="../../methods/idiademcalculationchannel-xrelation/">XRelation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addcalculationchannel/">AddCalculationChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addcalculationchannelref/">AddCalculationChannelRef</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addchannel/">AddChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-item/">Item</a> | <a href="../inavidata/">Data</a>.<a href="../../methods/inavidata-getchannel/">GetChannel</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademCalculationChannel.htm`*

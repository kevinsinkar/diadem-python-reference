---
title: "IDiademAssignmentChannel"
description: "The AssignmentChannel object provides an assignment channel in the script interface for internal data."
---

# IDiademAssignmentChannel

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: AssignmentChannel <Data>

The AssignmentChannel object provides an assignment channel in the script interface for internal data.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Assignment channels do not support assignments to time values.</td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value", dd.DataTypeChnFloat64, 1)
if oMyChn.IsKindOf(dd.eDataAssignmentChannel) :
    dd.MsgBoxDisp("assignment channel")
else:
    dd.MsgBoxDisp("no assignment channel")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademassignmentchannel-assignmentlist/">AssignmentList</a> | <a href="../../properties/idiademassignmentchannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/idiademassignmentchannel-datatype/">DataType</a> | <a href="../../properties/idiademassignmentchannel-defaultvalue/">DefaultValue</a> | <a href="../../properties/idiademassignmentchannel-dvalues/">dValues</a> | <a href="../../properties/idiademassignmentchannel-isreadonly/">IsReadOnly</a> | <a href="../../properties/idiademassignmentchannel-maximum/">Maximum</a> | <a href="../../properties/idiademassignmentchannel-minimum/">Minimum</a> | <a href="../../properties/idiademassignmentchannel-name/">Name</a> | <a href="../../properties/idiademassignmentchannel-novalues/">NoValues</a> | <a href="../../properties/idiademassignmentchannel-operationalflags/">OperationalFlags</a> | <a href="../../properties/idiademassignmentchannel-properties/">Properties</a> | <a href="../../properties/idiademassignmentchannel-reservedsize/">ReservedSize</a> | <a href="../../properties/idiademassignmentchannel-size/">Size</a> | <a href="../../properties/idiademassignmentchannel-unitsymbol/">UnitSymbol</a> | <a href="../../properties/idiademassignmentchannel-valueindex/">ValueIndex</a> | <a href="../../properties/idiademassignmentchannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademassignmentchannel-getreference/">GetReference</a> | <a href="../../methods/idiademassignmentchannel-getvaluesblock/">GetValuesBlock</a> | <a href="../../methods/idiademassignmentchannel-iskindof/">IsKindOf</a> | <a href="../../methods/idiademassignmentchannel-removevalues/">RemoveValues</a> | <a href="../../methods/idiademassignmentchannel-setvalues/">SetValues</a> | <a href="../../methods/idiademassignmentchannel-setvaluesblock/">SetValuesBlock</a> | <a href="../../methods/idiademassignmentchannel-xrelation/">XRelation</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addassignmentchannel/">AddAssignmentChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-addchannel/">AddChannel</a> | <a href="../../collections/channels/">Channels &lt;Data&gt;</a>.<a href="../../methods/idiademchannels-item/">Item</a> | <a href="../inavidata/">Data</a>.<a href="../../methods/inavidata-getchannel/">GetChannel</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-add/">Add</a> | <a href="../../collections/elementlist/">ElementList &lt;Data&gt;</a>.<a href="../../methods/idiademelementlist-item/">Item</a> | <a href="../idiademproperty/">Property &lt;Data&gt;</a>.<a href="../../properties/idiademproperty-element/">Element</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademAssignmentChannel.htm`*

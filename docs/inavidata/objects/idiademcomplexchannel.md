---
title: "IDiademComplexChannel"
description: "ComplexChannel <Data> object provides a complex channel in the script interface for internal data. The Channel object is an element of the Channels collection. "
---

# IDiademComplexChannel

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: ComplexChannel <Data>

ComplexChannel <Data> object provides a complex channel in the script interface for internal data. The Channel object is an element of the Channels collection. Complex channels are a preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change.

## Python example

```python
oMyElement = dd.Portal.ActiveView.Selection(1)
if oMyElement.IsKindOf(dd.eDataComplexChannel) :
    dd.MsgBoxDisp("Property name: " + oMyElement.Name + "\r\n" + "Property unit: " + oMyElement.UnitSymbol)
else:
    dd.MsgBoxDisp ("Selected element is no complex channel")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idiademcomplexchannel-channelgroup/">ChannelGroup</a> | <a href="../../properties/idiademcomplexchannel-datatype/">DataType</a> | <a href="../../properties/idiademcomplexchannel-isreadonly/">IsReadOnly</a> | <a href="../../properties/idiademcomplexchannel-maximum/">Maximum</a> | <a href="../../properties/idiademcomplexchannel-minimum/">Minimum</a> | <a href="../../properties/idiademcomplexchannel-name/">Name</a> | <a href="../../properties/idiademcomplexchannel-novalues/">NoValues</a> | <a href="../../properties/idiademcomplexchannel-operationalflags/">OperationalFlags</a> | <a href="../../properties/idiademcomplexchannel-properties/">Properties</a> | <a href="../../properties/idiademcomplexchannel-reservedsize/">ReservedSize</a> | <a href="../../properties/idiademcomplexchannel-unitsymbol/">UnitSymbol</a> | <a href="../../properties/idiademcomplexchannel-valueindex/">ValueIndex</a> | <a href="../../properties/idiademcomplexchannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idiademcomplexchannel-getreference/">GetReference</a> | <a href="../../methods/idiademcomplexchannel-getvaluesblock/">GetValuesBlock</a> | <a href="../../methods/idiademcomplexchannel-iskindof/">IsKindOf</a> | <a href="../../methods/idiademcomplexchannel-removevalues/">RemoveValues</a> | <a href="../../methods/idiademcomplexchannel-setvalues/">SetValues</a> | <a href="../../methods/idiademcomplexchannel-setvaluesblock/">SetValuesBlock</a> | <a href="../../methods/idiademcomplexchannel-xrelation/">XRelation</a></p>
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

*Source: `Inavidata/objects/DiaCmpnt_Objects_IDiademComplexChannel.htm`*

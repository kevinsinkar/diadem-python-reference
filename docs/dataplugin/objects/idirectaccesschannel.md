---
title: "IDirectAccessChannel"
description: "The DirectAccessChannel object provides access to a DirectAccess channel and the associated properties."
---

# IDirectAccessChannel

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: DirectAccessChannel

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The DirectAccessChannel object provides access to a DirectAccess channel and the associated properties.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyChn.Factor = 2
oMyChn.Offset = 5
```

```python
for i in range(1, oCurrSheet.MaxPosition.Column + 1):
    Name = oCurrSheet.GetCellValue(1,i)
    oNewChannel = oCellBlock.Channels.Add(Name)
    Root.ChannelGroups(1).Channels.AddDirectAccessChannel(oNewChannel)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idirectaccesschannel-datatype/">DataType</a> | <a href="../../properties/idirectaccesschannel-factor/">Factor</a> | <a href="../../properties/idirectaccesschannel-formatter/">Formatter</a> | <a href="../../properties/idirectaccesschannel-index/">Index</a> | <a href="../../properties/idirectaccesschannel-name/">Name</a> | <a href="../../properties/idirectaccesschannel-offset/">Offset</a> | <a href="../../properties/idirectaccesschannel-properties/">Properties</a> | <a href="../../properties/idirectaccesschannel-size/">Size</a> | <a href="../../properties/idirectaccesschannel-values/">Values</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idirectaccesschannel-addcharacteristics/">AddCharacteristics</a> | <a href="../../methods/idirectaccesschannel-addwaveformproperties/">AddWaveformProperties</a> | <a href="../../methods/idirectaccesschannel-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/abstractdirectaccesschannels/">AbstractDirectAccessChannels</a>.<a href="../../methods/iabstractdirectaccesschannels-item/">Item</a> | <a href="../../collections/binarydirectaccesschannels/">BinaryDirectAccessChannels</a>.<a href="../../methods/ibinarydirectaccesschannels-add/">Add</a> | <a href="../../collections/binarydirectaccesschannels/">BinaryDirectAccessChannels</a>.<a href="../../methods/ibinarydirectaccesschannels-item/">Item</a> | <a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-adddirectaccesschannel/">AddDirectAccessChannel</a> | <a href="../../collections/channels/">Channels &lt;DataPlugin&gt;</a>.<a href="../../methods/ichannels-item/">Item</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-add/">Add</a> | <a href="../../collections/channelstoprocess/">ChannelsToProcess</a>.<a href="../../methods/ichannelstoprocess-item/">Item</a> | <a href="../../collections/directaccesschannels/">DirectAccessChannels</a>.<a href="../../methods/idirectaccesschannels-add/">Add</a> | <a href="../../collections/directaccesschannels/">DirectAccessChannels</a>.<a href="../../methods/idirectaccesschannels-item/">Item</a> | <a href="../../collections/directcellchannels/">DirectCellChannels</a>.<a href="../../methods/iexceldachannels-add/">Add</a> | <a href="../../collections/directcellchannels/">DirectCellChannels</a>.<a href="../../methods/iexceldachannels-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IDirectAccessChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

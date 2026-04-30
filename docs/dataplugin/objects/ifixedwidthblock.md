---
title: "IFixedWidthBlock"
description: "Use the FixedWidthBlock object to access channel data in a text file."
---

# IFixedWidthBlock

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: FixedWidthBlock

Use the FixedWidthBlock object to access channel data in a text file.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The file pointer of the text file does not move when a FixedWidthBlock is read out.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oChn1.Formatter.CharacterCount = 4
oChn1.Formatter.SampleWidth = 2

oChannelGroup.Channels.AddDirectAccessChannel(oChn1)

oBlock.Position = File.Position
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ifixedwidthblock-blocklength/">BlockLength</a> | <a href="../../properties/ifixedwidthblock-channels/">Channels</a> | <a href="../../properties/ifixedwidthblock-position/">Position</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ifixedwidthblock-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../imeasurementfileio/">File</a>.<a href="../../methods/imeasurementfileio-getfixedwidthblock/">GetFixedWidthBlock</a> | <a href="../ifixedwidthchannelformatter/">FixedWidthChannelFormatter</a>.<a href="../../properties/ifixedwidthchannelformatter-block/">Block</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IFixedWidthBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

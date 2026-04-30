---
title: "IStringBlock"
description: "The StringBlock object facilitates access to text, single values, and channel data in a text file."
---

# IStringBlock

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: StringBlock

The StringBlock object facilitates access to text, single values, and channel data in a text file.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The file pointer of the text file does not move when a StringBlock is read.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyGrp.Channels.AddDirectAccessChannel(oChn1)
oMyGrp.Channels.AddDirectAccessChannel(oChn2)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/istringblock-blocklength/">BlockLength</a> | <a href="../../properties/istringblock-channels/">Channels</a> | <a href="../../properties/istringblock-position/">Position</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/istringblock-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../imeasurementfileio/">File</a>.<a href="../../methods/imeasurementfileio-getstringblock/">GetStringBlock</a> | <a href="../istringchannelformatter/">StringChannelFormatter</a>.<a href="../../properties/istringchannelformatter-block/">Block</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IStringBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

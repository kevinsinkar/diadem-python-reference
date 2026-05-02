---
title: "IAbstractChannelFormatter"
description: "The AbstractChannelFormatter object contains information about how the values of a channel are represented in the file."
---

# IAbstractChannelFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: AbstractChannelFormatter

The AbstractChannelFormatter object contains information about how the values of a channel are represented in the file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in oBlock.Channels:
    if oMyChn.Formatter.IsKindOf(eStringBlock):
        oMyChn.Properties.Add("BlockType", "StringBlock")
    elif oMyChn.Formatter.IsKindOf(eBinaryBlock):
        oMyChn.Properties.Add("BlockType", "BinaryBlock")
    elif oMyChn.Formatter.IsKindOf(eFixedWidthBlock):
        oMyChn.Properties.Add("BlockType", "FixedWidthBlock")
    elif oMyChn.Formatter.IsKindOf(eCellBlock):
        oMyChn.Properties.Add("BlockType", "CellBlock")
```

## Members

<div markdown="1">
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iabstractchannelformatter-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idirectaccesschannel/">DirectAccessChannel</a>.<a href="../../properties/idirectaccesschannel-formatter/">Formatter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IAbstractChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

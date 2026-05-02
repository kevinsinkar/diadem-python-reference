---
title: "IAbstractChannelFormatter.IsKindOf"
description: "Checks whether the AbstractChannelFormatter object is a certain type. The AbstractChannelFormatter object contains information about how the values of a channel"
---

# IAbstractChannelFormatter.IsKindOf

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: IsKindOf for AbstractChannelFormatter

Checks whether the AbstractChannelFormatter object is a certain type. The AbstractChannelFormatter object contains information about how the values of a channel are represented in the file. Depending on whether the channel belongs to a BinaryBlock, StringBlock, FixedWidthBlock, or CellBlock the AbstractChannelFormatter is a BinaryChannelFormatter , StringChannelFormatter , FixedWidthChannelFormatter , or CellChannelFormatter object.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_IsKindOf_IAbstractChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

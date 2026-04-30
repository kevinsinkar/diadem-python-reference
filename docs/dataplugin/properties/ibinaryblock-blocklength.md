---
title: "IBinaryBlock.BlockLength"
description: "Specifies the number of values that a channel in the BinaryBlock contains. If the number is -1 , the block extends to the end of the file."
---

# IBinaryBlock.BlockLength

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: BlockLength for BinaryBlock

Specifies the number of values that a channel in the BinaryBlock contains. If the number is -1 , the block extends to the end of the file.

## Signature

```python
obj.BlockLength
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if oBlock.IsKindOf(eBinaryBlock):
    oBlock.BlockLength = -1
else:
    oBlock.BlockLength = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_BlockLength_IBinaryBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

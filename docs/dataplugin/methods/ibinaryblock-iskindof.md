---
title: "IBinaryBlock.IsKindOf"
description: "Checks whether a BinaryBlock object is a certain type."
---

# IBinaryBlock.IsKindOf

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: IsKindOf for BinaryBlock

Checks whether a BinaryBlock object is a certain type.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if oBlock.IsKindOf(eBinaryBlock):
    oBlock.BlockLength = -1
elif oBlock.IsKindOf(eFixedWidthBlock):
    oBlock.BlockLength = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_IsKindOf_IBinaryBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

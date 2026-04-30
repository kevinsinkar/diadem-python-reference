---
title: "IStringBlock.IsKindOf"
description: "Checks whether a StringBlock object is a certain type."
---

# IStringBlock.IsKindOf

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: IsKindOf for StringBlock

Checks whether a StringBlock object is a certain type.

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
    ElseIf oBlock.IsKindOf(eStringBlock) :
    oBlock.BlockLength = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_IsKindOf_IStringBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

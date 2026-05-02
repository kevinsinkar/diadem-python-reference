---
title: "IStringBlock.BlockLength"
description: "Specifies the number of values that a channel in the StringBlock contains. If the number is -1 , the block extends to the end of the file."
---

# IStringBlock.BlockLength

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: BlockLength for StringBlock

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the number of values that a channel in the StringBlock contains. If the number is -1 , the block extends to the end of the file.

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
elif oBlock.IsKindOf(eStringBlock):
    oBlock.BlockLength = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_BlockLength_IStringBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

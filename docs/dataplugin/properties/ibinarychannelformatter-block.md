---
title: "IBinaryChannelFormatter.Block"
description: "Contains the parent object for a BinaryChannelFormatter object."
---

# IBinaryChannelFormatter.Block

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Block for BinaryChannelFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Contains the parent object for a BinaryChannelFormatter object.

## Signature

```python
return_value = obj.Block
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if oMyChn.Formatter.Block.IsKindOf(eBinaryBlock):
    oMyChn.Formatter.ByteOrder = eBigEndian
```

## See also

<div markdown="1">
<div class="SeeAlso">
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_Property_Block_IBinaryChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IBinaryChannelFormatter.BitMask"
description: "Specifies the bit mask that masks the value DIAdem reads in."
---

# IBinaryChannelFormatter.BitMask

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: BitMask for BinaryChannelFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the bit mask that masks the value DIAdem reads in.

## Signature

```python
obj.BitMask
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The bit mask is ignored when R32 values and R64 values are read.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>You can specify the value of the bit mask as a decimal, hexadecimal, or octal. <span class="Monospace">1234</span> is a decimal value, <span class="Monospace">0x134</span> is a hexadecimal value, and <span class="Monospace">01234</span> is an octal value.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oChn.Formatter.Bitmask = 16
oChn.Factor = 0.0625
oMyGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso">
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_Property_BitMask_IBinaryChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

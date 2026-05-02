---
title: "IDirectAccessChannels.Swap"
description: "Moves an DirectAccess channel to a specific position."
---

# IDirectAccessChannels.Swap

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Swap for DirectAccessChannels

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Moves an DirectAccess channel to a specific position.

## Signature

```python
obj.Swap(Index1, Index2)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oBlock.Channels.Swap(oBlock.Channels.Item("YShift").Index, oBlock.Channels.Item("XShift").Index)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Swap_IDirectAccessChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

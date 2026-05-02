---
title: "IDirectAccessChannel.Values"
description: "Returns the single value of a DirectAccessChannel at a specific channel position."
---

# IDirectAccessChannel.Values

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Values for DirectAccessChannel

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the single value of a DirectAccessChannel at a specific channel position.

## Signature

```python
obj.Values(Index)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, oChn.Size + 1):
    Sum = Sum + oChn.Values(i)
oChn.Properties.Add("Sum",Sum)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Root Object Overview</a> | <a href="#" data-unresolved="1">File Object Overview</a> | <a href="#" data-unresolved="1">Workbook Object Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Values_IDirectAccessChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

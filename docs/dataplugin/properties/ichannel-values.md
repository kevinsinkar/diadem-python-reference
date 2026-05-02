---
title: "IChannel.Values"
description: "Contains the single value of a channel at a specific channel position."
---

# IChannel.Values

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Values for Channel <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Contains the single value of a channel at a specific channel position.

## Signature

```python
obj.Values(iIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  The <span class="Monospace">Size</span> property contains the current number of values of a channel.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Channel values that are not set receive the NoValue value. The NoValue value is <span class="Monospace">Null</span> in VBS. Use the <span class="Monospace">IsNull</span> function to carry out comparisons with the <span class="Monospace">Null</span> value.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, 100 + 1):
    oMyChn.Values(i) = CDbl(i/100000)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Values_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

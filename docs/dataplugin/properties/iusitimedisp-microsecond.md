---
title: "IUsiTimeDisp.Microsecond"
description: "Specifies the microseconds."
---

# IUsiTimeDisp.Microsecond

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Microsecond for UsiTimeDisp

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the microseconds.

## Signature

```python
obj.Microsecond
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.Properties.Add("Microsecond", oMyTime.Microsecond)
```

---

*Source: `DataPlugin/Properties/DataPlugin_property_Microsecond_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

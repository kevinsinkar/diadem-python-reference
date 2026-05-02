---
title: "IUsiTimeDisp.VariantDate"
description: "Specifies a date or time. This entry does not include microseconds and nanoseconds."
---

# IUsiTimeDisp.VariantDate

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: VariantDate for UsiTimeDisp

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies a date or time. This entry does not include microseconds and nanoseconds.

## Signature

```python
return_value = obj.VariantDate
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyTime = CreateTime(2013,9,13,10,51,44,123,456,789)
oMyTime.VariantDate = NOW
dd.Data.Root.Properties.Add("DateTime", oMyTime)
```

---

*Source: `DataPlugin/Properties/DataPlugin_property_VariantDate_IUsiTimeDisp.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IUsiTimeDisp.VariantDate"
description: "Specifies a date or time. This entry does not include microseconds and nanoseconds."
---

# IUsiTimeDisp.VariantDate

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: VariantDate for UsiTimeDisp

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

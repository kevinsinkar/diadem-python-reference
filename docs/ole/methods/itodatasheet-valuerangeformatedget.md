---
title: "ITODataSheet.ValueRangeFormatedGet"
description: "Reads out a data range of the DIAdem values matrix and returns this range, formatted, as a variant or a string."
---

# ITODataSheet.ValueRangeFormatedGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ValueRangeFormatedGet for TODataSheet

Reads out a data range of the DIAdem values matrix and returns this range, formatted, as a variant or a string.

## Signature

```python
iValueRangeFormatedGet = Object.ValueRangeFormatedGet(nStartRowV, vStartChnV, nEndRowV, vEndChnV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ValueRangeFormatedGet(1,"Time",500,"Torque",vValueP)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ValueRangeFormatedGet_ITODataSheet.htm`*

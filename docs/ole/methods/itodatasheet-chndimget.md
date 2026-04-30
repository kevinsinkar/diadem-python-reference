---
title: "ITODataSheet.ChnDimGet"
description: "Reads a channel unit."
---

# ITODataSheet.ChnDimGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnDimGet for TODataSheet

Reads a channel unit.

## Signature

```python
iChnDimGet = Object.ChnDimGet(vChnV, vDimensionP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnDimGet("Time",vUnitP)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnDimGet_ITODataSheet.htm`*

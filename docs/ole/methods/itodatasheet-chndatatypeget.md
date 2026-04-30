---
title: "ITODataSheet.ChnDataTypeGet"
description: "Reads the channel data type."
---

# ITODataSheet.ChnDataTypeGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnDataTypeGet for TODataSheet

Reads the channel data type.

## Signature

```python
iChnDataTypeGet = Object.ChnDataTypeGet(vChnV, vDataTypeP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnDataTypeGet("Time", vDataTypeP)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnDataTypeGet_ITODataSheet.htm`*

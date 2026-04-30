---
title: "ITODataSheet.ChnNameGet"
description: "Reads a channel name."
---

# ITODataSheet.ChnNameGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnNameGet for TODataSheet

Reads a channel name.

## Signature

```python
iChnNameGet = Object.ChnNameGet(vChnV, vNameP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnNameGet(5,vNameV)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnNameGet_ITODataSheet.htm`*

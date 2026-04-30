---
title: "ITODataSheet.ChnValGet"
description: "Reads a single channel value."
---

# ITODataSheet.ChnValGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnValGet for TODataSheet

Reads a single channel value.

## Signature

```python
iChnValGet = Object.ChnValGet(nRowV, vChnV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    for lCountT in range( 1, 10+1):
        iSuccess = oDIAdem.ChnValGet(lCountT,"Time", vValueP)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnValGet_ITODataSheet.htm`*

---
title: "ITODataSheet.ChnLengthGet"
description: "Reads the channel length."
---

# ITODataSheet.ChnLengthGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnLengthGet for TODataSheet

Reads the channel length.

## Signature

```python
iChnLengthGet = Object.ChnLengthGet(vChnV, vLengthP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.MaxChnLengthGet(1,vMaxLengthP)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnLengthGet_ITODataSheet.htm`*

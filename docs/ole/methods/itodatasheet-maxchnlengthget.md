---
title: "ITODataSheet.MaxChnLengthGet"
description: "Reads the maximum valid channel length."
---

# ITODataSheet.MaxChnLengthGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: MaxChnLengthGet for TODataSheet

Reads the maximum valid channel length.

## Signature

```python
iMaxChnLengthGet = Object.MaxChnLengthGet(vChnV, vMaxLengthP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.MaxChnLengthGet("Time",vMaxLengthP)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_MaxChnLengthGet_ITODataSheet.htm`*

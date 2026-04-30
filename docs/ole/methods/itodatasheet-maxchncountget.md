---
title: "ITODataSheet.MaxChnCountGet"
description: "Reads the maximum valid number of channels."
---

# ITODataSheet.MaxChnCountGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: MaxChnCountGet for TODataSheet

Reads the maximum valid number of channels.

## Signature

```python
iMaxChnCountGet = Object.MaxChnCountGet(vCountV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.MaxChnCountGet(vMaxCountP)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_MaxChnCountGet_ITODataSheet.htm`*

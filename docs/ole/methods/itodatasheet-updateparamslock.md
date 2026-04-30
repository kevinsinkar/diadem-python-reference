---
title: "ITODataSheet.UpdateParamsLock"
description: "Activates or deactivates the automatic updating of the channel characteristic values when the channel values are modified."
---

# ITODataSheet.UpdateParamsLock

!!! abstract "Method &middot; `OLE.chm`"
    Method: UpdateParamsLock for TODataSheet

Activates or deactivates the automatic updating of the channel characteristic values when the channel values are modified.

## Signature

```python
iUpdateParamsLock = Object.UpdateParamsLock(nStateV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.UpdateParamsLock(1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_UpdateParamsLock_ITODataSheet.htm`*

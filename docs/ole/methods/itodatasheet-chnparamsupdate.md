---
title: "ITODataSheet.ChnParamsUpdate"
description: "Refreshes the characteristic values of channels."
---

# ITODataSheet.ChnParamsUpdate

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnParamsUpdate for TODataSheet

Refreshes the characteristic values of channels.

## Signature

```python
iChnParamsUpdate = Object.ChnParamsUpdate(vStartChnV, vEndChnV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnParamsUpdate(1,12)
#Using channel names:
    iSuccess = oDIAdem.ChnParamsUpdate("Time", "Torque")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnParamsUpdate_ITODataSheet.htm`*

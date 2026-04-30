---
title: "ITODataSheet.ChnLengthSet"
description: "Sets the channel length."
---

# ITODataSheet.ChnLengthSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnLengthSet for TODataSheet

Sets the channel length.

## Signature

```python
iChnLengthSet = Object.ChnLengthSet(vChnV, nLengthV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnLengthSet("Time",10)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnLengthSet_ITODataSheet.htm`*

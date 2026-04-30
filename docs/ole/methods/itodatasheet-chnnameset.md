---
title: "ITODataSheet.ChnNameSet"
description: "Sets a channel name."
---

# ITODataSheet.ChnNameSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnNameSet for TODataSheet

Sets a channel name.

## Signature

```python
iChnNameSet = Object.ChnNameSet(vChnV, sgNameV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnNameSet("Time","NewTime")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnNameSet_ITODataSheet.htm`*

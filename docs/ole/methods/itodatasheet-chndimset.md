---
title: "ITODataSheet.ChnDimSet"
description: "Sets the unit in a channel."
---

# ITODataSheet.ChnDimSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnDimSet for TODataSheet

Sets the unit in a channel.

## Signature

```python
iChnDimSet = Object.ChnDimSet(vChnV, sgDimensionV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnDimSet("Time","s")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnDimSet_ITODataSheet.htm`*

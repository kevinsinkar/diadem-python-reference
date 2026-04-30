---
title: "ITODataSheet.bInterfaceLocked"
description: "Requests the status of the OLE interfaces from DIAdem. Always request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an "
---

# ITODataSheet.bInterfaceLocked

!!! abstract "Property &middot; `OLE.chm`"
    Property: bInterfaceLocked for TODataSheet

Requests the status of the OLE interfaces from DIAdem. Always request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an OLE command to DIAdem although the property has the value True , the behavior of DIAdem is unpredictable.

## Signature

```python
obj.bInterfaceLocked
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
while True:
    if not oDIAdem.bInterfaceLocked:
            break
iSuccess = oDIAdem.ChnCommentGet(5, vCommentP)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/properties/OLE_property_bInterfaceLocked_ITODataSheet.htm`*

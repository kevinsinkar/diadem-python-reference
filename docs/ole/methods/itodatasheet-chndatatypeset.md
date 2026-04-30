---
title: "ITODataSheet.ChnDataTypeSet"
description: "Sets the display format of a channel."
---

# ITODataSheet.ChnDataTypeSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnDataTypeSet for TODataSheet

Sets the display format of a channel.

## Signature

```python
iChnDataTypeSet = Object.ChnDataTypeSet(vChnV, DataTypeV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem. ChnDataTypeSet("Time", "Numeric")
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnDataTypeSet_ITODataSheet.htm`*

---
title: "ITODataSheet.ValueRangeFormatedSet"
description: "Sets a data area in DIAdem."
---

# ITODataSheet.ValueRangeFormatedSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ValueRangeFormatedSet for TODataSheet

Sets a data area in DIAdem.

## Signature

```python
iValueRangeFormatedSet = Object.ValueRangeFormatedSet(nStartRowV, vStartChnV, nEndRowV, vEndChnV, vValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    vValueV = [[4711 for _ in range(4)] for _ in range(500)]
    iSuccess = oDIAdem.ValueRangeFormatedSet(1, "Time", 500, "Torque", vValueV)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ValueRangeFormatedSet_ITODataSheet.htm`*

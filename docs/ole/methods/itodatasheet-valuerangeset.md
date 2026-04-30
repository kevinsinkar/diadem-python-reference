---
title: "ITODataSheet.ValueRangeSet"
description: "Sets values in DIAdem channels."
---

# ITODataSheet.ValueRangeSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ValueRangeSet for TODataSheet

Sets values in DIAdem channels.

## Signature

```python
iValueRangeSet = Object.ValueRangeSet(nStartRowV, vStartChnV, nEndRowV, vEndChnV, vValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    vValueV = [[4711 for _ in range(4)] for _ in range(500)]
    iSuccess = oDIAdem.ValueRangeSet(1, "Time", 500, "Torque", vValueV)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ValueRangeSet_ITODataSheet.htm`*

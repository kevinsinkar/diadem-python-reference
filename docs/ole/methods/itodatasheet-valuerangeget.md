---
title: "ITODataSheet.ValueRangeGet"
description: "Reads out data values from a range in the DIAdem channels."
---

# ITODataSheet.ValueRangeGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ValueRangeGet for TODataSheet

Reads out data values from a range in the DIAdem channels.

## Signature

```python
iValueRangeGet = Object.ValueRangeGet(nStartRowV, vStartChnV, nEndRowV, vEndChnV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet") #
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ValueRangeGet(1,"[1]/Speed",500,"[1]/Revs", vValue)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ValueRangeGet_ITODataSheet.htm`*

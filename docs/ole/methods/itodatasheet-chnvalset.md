---
title: "ITODataSheet.ChnValSet"
description: "Sets a single channel value."
---

# ITODataSheet.ChnValSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: ChnValSet for TODataSheet

Sets a single channel value.

## Signature

```python
iChnValSet = Object.ChnValSet(nRowV, vChnV, vValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
if not oDIAdem.bInterfaceLocked :
    for lCountT in range( 1, 10+1):
        iSuccess = oDIAdem.ChnValSet(lCountT,"Time", lCountT*10)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_ChnValSet_ITODataSheet.htm`*

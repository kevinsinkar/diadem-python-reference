---
title: "ITODataSheet.bNoActivityDisplay"
description: "Suppresses the DIAdem Tray icon. This is useful if you want to operate DIAdem as a server and achieve the highest possible performance."
---

# ITODataSheet.bNoActivityDisplay

!!! abstract "Property &middot; `OLE.chm`"
    Property: bNoActivityDisplay for TODataSheet

Suppresses the DIAdem Tray icon. This is useful if you want to operate DIAdem as a server and achieve the highest possible performance.

## Signature

```python
obj.bNoActivityDisplay
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
oDIAdem.bNoActivityDisplay = True
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.ChnCommentSet("Time","Comment")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/properties/OLE_property_bNoActivityDisplay_ITODataSheet.htm`*

---
title: "ITODataSheet.bNoMsgDisplay"
description: "Suppresses all DIAdem message boxes and dialog boxes. This behavior is useful if you want to operate DIAdem as a server."
---

# ITODataSheet.bNoMsgDisplay

!!! abstract "Property &middot; `OLE.chm`"
    Property: bNoMsgDisplay for TODataSheet

Suppresses all DIAdem message boxes and dialog boxes. This behavior is useful if you want to operate DIAdem as a server.

## Signature

```python
obj.bNoMsgDisplay
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TODataSheet")
oDIAdem.bNoMsgDisplay = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/properties/OLE_property_bNoMsgDisplay_ITODataSheet.htm`*

---
title: "ITOCommand.bDontCloseApplication"
description: "Prevents DIAdem from closing automatically after DIAdem ends the OLE connection."
---

# ITOCommand.bDontCloseApplication

!!! abstract "Property &middot; `OLE.chm`"
    Property: bDontCloseApplication for TOCommand

Prevents DIAdem from closing automatically after DIAdem ends the OLE connection.

## Signature

```python
obj.bDontCloseApplication
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
oDIAdem.bDontCloseApplication = True
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.CmdExecuteSync("MsgBoxDisp('Hello World')")
    iSuccess = oDIAdem.CmdExecuteSync("wndshow('shell','normal')")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/properties/OLE_property_bDontCloseApplication_ITOCommand.htm`*

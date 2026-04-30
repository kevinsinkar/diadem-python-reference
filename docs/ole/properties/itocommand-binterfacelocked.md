---
title: "ITOCommand.bInterfaceLocked"
description: "Requests the status of the OLE interfaces from DIAdem. Always request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an "
---

# ITOCommand.bInterfaceLocked

!!! abstract "Property &middot; `OLE.chm`"
    Property: bInterfaceLocked for TOCommand

Requests the status of the OLE interfaces from DIAdem. Always request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an OLE command to DIAdem although the property has the value True , the behavior of DIAdem is unpredictable.

## Signature

```python
obj.bInterfaceLocked
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
oDIAdem.bNoActivityDisplay = True
if not oDIAdem.bInterfaceLocked :
#Initialize TOCommand Interface:
    while True:
        if not oDIAdem.bInterfaceLocked:
                break
    iSuccess = oDIAdem.CmdExecuteSync("wndshow('shell','normal')")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/properties/OLE_property_bInterfaceLocked_ITOCommand.htm`*

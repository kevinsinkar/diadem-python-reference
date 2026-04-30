---
title: "ITOCommand.CmdExecuteSync"
description: "Executes a DIAdem command synchronously. The program does not continue until DIAdem has completely performed the command."
---

# ITOCommand.CmdExecuteSync

!!! abstract "Method &middot; `OLE.chm`"
    Method: CmdExecuteSync for TOCommand

Executes a DIAdem command synchronously. The program does not continue until DIAdem has completely performed the command.

## Signature

```python
iCmdExecuteSync = Object.CmdExecuteSync(vCmdV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.CmdExecuteSync("wndshow('shell','normal')")
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_CmdExecuteSync_ITOCommand.htm`*

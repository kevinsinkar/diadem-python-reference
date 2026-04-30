---
title: "ITOCommand.CmdExecuteAsync"
description: "Executes a DIAdem command asynchronously. The program continues immediately, while DIAdem is performing the command."
---

# ITOCommand.CmdExecuteAsync

!!! abstract "Method &middot; `OLE.chm`"
    Method: CmdExecuteAsync for TOCommand

Executes a DIAdem command asynchronously. The program continues immediately, while DIAdem is performing the command.

## Signature

```python
iCmdExecuteAsync = Object.CmdExecuteAsync(vCmdV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.CmdExecuteASync("wndshow('shell','normal')")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_CmdExecuteAsync_ITOCommand.htm`*

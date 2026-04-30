---
title: "ITOCommand.TextVarGet"
description: "Reads out a DIAdem variable."
---

# ITOCommand.TextVarGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: TextVarGet for TOCommand

Reads out a DIAdem variable.

## Signature

```python
iTextVarGet = Object.TextVarGet(sgVarNameV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.TextVarGet("DataReadPath", vDataReadPathP)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_TextVarGet_ITOCommand.htm`*

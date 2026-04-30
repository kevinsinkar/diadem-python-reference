---
title: "ITOCommand.BoolVarGet"
description: "Reads out a Boolean DIAdem variable."
---

# ITOCommand.BoolVarGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: BoolVarGet for TOCommand

Reads out a Boolean DIAdem variable.

## Signature

```python
iBoolVarGet = Object.BoolVarGet(sgVarNameV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.BoolVarGet("B1", vB1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_BoolVarGet_ITOCommand.htm`*

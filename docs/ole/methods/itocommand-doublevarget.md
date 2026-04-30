---
title: "ITOCommand.DoubleVarGet"
description: "Reads out a DIAdem variable."
---

# ITOCommand.DoubleVarGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: DoubleVarGet for TOCommand

Reads out a DIAdem variable.

## Signature

```python
iDoubleVarGet = Object.DoubleVarGet(sgVarNameV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.DoubleVarGet("R1", vR1P)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_DoubleVarGet_ITOCommand.htm`*

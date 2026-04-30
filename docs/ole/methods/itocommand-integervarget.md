---
title: "ITOCommand.IntegerVarGet"
description: "Reads out a DIAdem variable."
---

# ITOCommand.IntegerVarGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: IntegerVarGet for TOCommand

Reads out a DIAdem variable.

## Signature

```python
iIntegerVarGet = Object.IntegerVarGet(sgVarNameV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
oDIAdem.bNoActivityDisplay = True
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.IntegerVarGet("SmoothWidth", vSmoothWidth)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_IntegerVarGet_ITOCommand.htm`*

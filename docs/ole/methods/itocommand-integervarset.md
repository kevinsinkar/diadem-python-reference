---
title: "ITOCommand.IntegerVarSet"
description: "Sets a DIAdem variable."
---

# ITOCommand.IntegerVarSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: IntegerVarSet for TOCommand

Sets a DIAdem variable.

## Signature

```python
iIntegerVarSet = Object.IntegerVarSet(sgVarNameV, vValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.IntegerVarSet("SmoothWidth",4)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_IntegerVarSet_ITOCommand.htm`*

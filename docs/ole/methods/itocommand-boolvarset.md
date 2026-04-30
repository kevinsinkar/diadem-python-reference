---
title: "ITOCommand.BoolVarSet"
description: "Sets a DIAdem variable."
---

# ITOCommand.BoolVarSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: BoolVarSet for TOCommand

Sets a DIAdem variable.

## Signature

```python
iBoolVarSet = Object.BoolVarSet(sgVarNameV, vValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.BoolVarSet("B1", True)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_BoolVarSet_ITOCommand.htm`*

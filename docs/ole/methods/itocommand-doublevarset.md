---
title: "ITOCommand.DoubleVarSet"
description: "Sets a DIAdem variable."
---

# ITOCommand.DoubleVarSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: DoubleVarSet for TOCommand

Sets a DIAdem variable.

## Signature

```python
iDoubleVarSet = Object.DoubleVarSet(sgVarNameV, vValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.DoubleVarSet("Novalue",9.9E+20)
    iSuccess = oDIAdem.DoubleVarSet("R1","NOVALUE")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_DoubleVarSet_ITOCommand.htm`*

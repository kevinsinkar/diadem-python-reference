---
title: "ITOCommand.TextVarSet"
description: "Sets a DIAdem variable."
---

# ITOCommand.TextVarSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: TextVarSet for TOCommand

Sets a DIAdem variable.

## Signature

```python
iTextVarSet = Object.TextVarSet(sgVarNameV, sgValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    lSuccess = oDIAdem.TextVarSet("DataReadPath","D:\\Projects")
```

## See also

<div markdown="1">
<div class="SeeAlso"> <h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_TextVarSet_ITOCommand.htm`*

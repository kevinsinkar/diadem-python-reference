---
title: "ITOCommand.NoValueSet"
description: "Sets the NoValue value in DIAdem."
---

# ITOCommand.NoValueSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: NoValueSet for TOCommand

Sets the NoValue value in DIAdem.

## Signature

```python
iNoValueSet = Object.NoValueSet(vNoValueV)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    vValueV = 4711
    iSuccess = oDIAdem.NoValueSet(vValueV)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_NoValueSet_ITOCommand.htm`*

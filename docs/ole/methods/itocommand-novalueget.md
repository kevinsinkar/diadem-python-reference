---
title: "ITOCommand.NoValueGet"
description: "Reads out the DIAdem NoValue value."
---

# ITOCommand.NoValueGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: NoValueGet for TOCommand

Reads out the DIAdem NoValue value.

## Signature

```python
iNoValueGet = Object.NoValueGet(vNoValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.NoValueGet(vValueP)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_NoValueGet_ITOCommand.htm`*

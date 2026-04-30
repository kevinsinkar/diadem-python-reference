---
title: "ITOCommand.VariantVarSet"
description: "Sets a variant type DIAdem variable. For example, you can use this method to access global user variables ."
---

# ITOCommand.VariantVarSet

!!! abstract "Method &middot; `OLE.chm`"
    Method: VariantVarSet for TOCommand

Sets a variant type DIAdem variable. For example, you can use this method to access global user variables .

## Signature

```python
iVariantVarSet = Object.VariantVarSet(sgVarNameV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    vVariant = "This could be an object"
    iSuccess = oDIAdem.VariantVarSet("O1", vVariant)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_VariantVarSet_ITOCommand.htm`*

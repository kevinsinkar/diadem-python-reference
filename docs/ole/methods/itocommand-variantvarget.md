---
title: "ITOCommand.VariantVarGet"
description: "Enables access to a DIAdem variant-type variable. For example, you can use the method to access a global user variable or DIAdem objects. DIAdem returns the val"
---

# ITOCommand.VariantVarGet

!!! abstract "Method &middot; `OLE.chm`"
    Method: VariantVarGet for TOCommand

Enables access to a DIAdem variant-type variable. For example, you can use the method to access a global user variable or DIAdem objects. DIAdem returns the value of the variable as a variant value.

## Signature

```python
iVariantVarGet = Object.VariantVarGet(sgVarNameV, vValueP)
```

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.VariantVarGet("VIEW", vVariant)
    print (vVariant.ActiveSheet.Name)
    VVariant.ActiveSheet.Name="MyName"
```

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
oDIAdem.bNoActivityDisplay = True
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.VariantVarGet("O1", vVariant)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/methods/OLE_method_VariantVarGet_ITOCommand.htm`*

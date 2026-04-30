---
title: "IValueUnit.IsKindOf"
description: "Checks whether the object is a certain type."
---

# IValueUnit.IsKindOf

!!! abstract "Method &middot; `IValueUnit.chm`"
    Method: IsKindOf for ValueWithUnit

Checks whether the object is a certain type.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Python example

```python
def Check(MyVar):
    if MyVar.IsKindOf(dd.eTypeValueUnit) :
        dd.MsgBoxDisp("ValueWithUnit object")
```

---

*Source: `IValueUnit/methods/DiaCmpnt_method_IsKindOf_IValueUnit.htm`*

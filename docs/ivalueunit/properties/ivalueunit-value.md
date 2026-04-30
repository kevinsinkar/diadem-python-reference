---
title: "IValueUnit.Value"
description: "Specifies the value of a value-unit object."
---

# IValueUnit.Value

!!! abstract "Property &middot; `IValueUnit.chm`"
    Property: Value for ValueWithUnit

Specifies the value of a value-unit object.

## Signature

```python
obj.Value
```

## Python example

```python
MyValueUnit = dd.CreateValueWithUnit(0.61, "m")
MyValueUnit.Convert("in")
dd.MsgBoxDisp(MyValueUnit.Value)
```

---

*Source: `IValueUnit/properties/DiaCmpnt_property_Value_IValueUnit.htm`*

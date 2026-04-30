---
title: "IValueUnit.Convert"
description: "Converts the previous unit of a value into a new unit. If you can convert the unit, DIAdem changes the properties Value and UnitSymbol of the specified value un"
---

# IValueUnit.Convert

!!! abstract "Method &middot; `IValueUnit.chm`"
    Method: Convert for ValueWithUnit

Converts the previous unit of a value into a new unit. If you can convert the unit, DIAdem changes the properties Value and UnitSymbol of the specified value unit object. If you cannot convert the unit, DIAdem displays an error message.

## Signature

```python
obj.Convert(TargetUnitSting)
```

## Python example

```python
MyValueUnit = dd.CreateValueWithUnit(0.61, "m")
MyValueUnit.Convert("in")
dd.MsgBoxDisp(MyValueUnit.Value)
```

---

*Source: `IValueUnit/methods/DiaCmpnt_method_Convert_IValueUnit.htm`*

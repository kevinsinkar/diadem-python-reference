---
title: "IValueUnit.UnitSymbol"
description: "Specifies the unit symbol of a value-unit object."
---

# IValueUnit.UnitSymbol

!!! abstract "Property &middot; `IValueUnit.chm`"
    Property: UnitSymbol for ValueWithUnit

Specifies the unit symbol of a value-unit object.

## Signature

```python
obj.UnitSymbol
```

## Python example

```python
MyValueUnit = dd.CreateValueWithUnit(0.61, "m")
MyValueUnit.Convert("in")
dd.MsgBoxDisp(MyValueUnit.Value + " " + MyValueUnit.UnitSymbol)
```

---

*Source: `IValueUnit/properties/DiaCmpnt_property_UnitSymbol_IValueUnit.htm`*

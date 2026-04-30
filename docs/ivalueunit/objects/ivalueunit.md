---
title: "IValueUnit"
description: "The ValueWithUnit object provides a value and a unit symbol. Use the DIAdem command CreateValueWithUnit to generate a value-unit object."
---

# IValueUnit

!!! abstract "Object &middot; `IValueUnit.chm`"
    Object: ValueWithUnit

The ValueWithUnit object provides a value and a unit symbol. Use the DIAdem command CreateValueWithUnit to generate a value-unit object.

## Python example

```python
MyValueUnit = dd.CreateValueWithUnit(0.61, "m")
MyValueUnit.Convert("in")
dd.MsgBoxDisp(MyValueUnit.Value + " " + MyValueUnit.UnitSymbol)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ivalueunit-unitsymbol/">UnitSymbol</a> | <a href="../../properties/ivalueunit-value/">Value</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ivalueunit-convert/">Convert</a> | <a href="../../methods/ivalueunit-iskindof/">IsKindOf</a></p>
</div>
</div>

---

*Source: `IValueUnit/objects/DiaCmpnt_Objects_IValueUnit.htm`*

---
title: "ITerminals.Count"
description: "Returns the number of VI terminals. A terminal is an input terminal or an output terminal of a VI."
---

# ITerminals.Count

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Count for Terminals

Returns the number of VI terminals. A terminal is an input terminal or an output terminal of a VI.

## Signature

```python
obj.Count
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
oMyTerminals = objVI.Terminals #Get Terminals
dd.MsgBoxDisp ("Number of Terminals: " + oMyTerminals.count)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/properties/LVHelper_property_Count_ITerminals.htm`*

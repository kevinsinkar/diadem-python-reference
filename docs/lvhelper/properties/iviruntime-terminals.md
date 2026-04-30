---
title: "IVIRuntime.Terminals"
description: "Returns a list of output terminals and input terminals of a VI."
---

# IVIRuntime.Terminals

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Terminals for VIRuntime

Returns a list of output terminals and input terminals of a VI.

## Signature

```python
return_value = obj.Terminals
```

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
oMyTerminals = objVI.Terminals #Get Terminals
strOutput = "List of terminals:"
for oMyTerminal in oMyTerminals:
    strOutput = strOutput + "\r\n" + "Name: " + oMyterminal.Name()
    strOutput = strOutput + ": Dimension is: " + dd.Str(oMyterminal.Dimensions())
    strOutput = strOutput + ": Type is: " + oMyterminal.Type()
    strOutput = strOutput + ": is output: " + oMyterminal.IsOut()
dd.MsgBoxDisp(strOutput)
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

*Source: `LVHelper/properties/LVHelper_property_Terminals_IVIRuntime.htm`*

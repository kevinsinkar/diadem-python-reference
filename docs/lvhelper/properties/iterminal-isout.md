---
title: "ITerminal.IsOut"
description: "Specifies whether a terminal is an output."
---

# ITerminal.IsOut

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: IsOut for Terminal

Specifies whether a terminal is an output.

## Signature

```python
obj.IsOut
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
    strOutput = strOutput + ": is output: " + oMyterminal.IsOut()
dd.MsgBoxDisp (strOutput)
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

*Source: `LVHelper/properties/LVHelper_property_IsOut_ITerminal.htm`*

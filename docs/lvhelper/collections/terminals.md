---
title: "Terminals"
description: "A list of all input terminals and output terminals of a VI."
---

# Terminals

!!! abstract "Collection &middot; `LVHelper.chm`"
    Collection: Terminals

A list of all input terminals and output terminals of a VI.

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
dd.MsgBoxDisp (strOutput)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

## Members

<div markdown="1">
<div class="Properties"><div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iterminals-count/">Count</a></p>
</div>
</div>
<div class="Methods"><div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iterminals-item/">Item</a></p>
</div>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/iviruntime/">VIRuntime</a>.<a href="../../properties/iviruntime-terminals/">Terminals</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/objects/LVHelper_Objects_ITerminals.htm`*

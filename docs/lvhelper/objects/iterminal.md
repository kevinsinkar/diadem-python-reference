---
title: "ITerminal"
description: "Returns a Terminal object. A terminal is an input terminal or an output terminal of a VI."
---

# ITerminal

!!! abstract "Object &middot; `LVHelper.chm`"
    Object: Terminal

Returns a Terminal object. A terminal is an input terminal or an output terminal of a VI.

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
oMyTerminals = objVI.Terminals #Get TerminalsDim strOutput
strOutput = "List of terminals:"
for oMyTerminal in oMyTerminals:
    strOutput = strOutput + "\r\n" + "Name: " + oMyTerminal.Name()
dd.MsgBoxDisp (strOutput)
# Clean upSet objVI = Nothing
dd.LVRuntime.DeInit()
```

## Members

<div markdown="1">
<div class="Properties"><div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iterminal-dimensions/">Dimensions</a> | <a href="../../properties/iterminal-isout/">IsOut</a> | <a href="../../properties/iterminal-name/">Name</a> | <a href="../../properties/iterminal-type/">Type</a></p>
</div>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/terminals/">Terminals</a>.<a href="../../methods/iterminals-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/objects/LVHelper_Objects_ITerminal.htm`*

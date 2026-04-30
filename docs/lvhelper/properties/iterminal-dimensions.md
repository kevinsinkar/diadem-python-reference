---
title: "ITerminal.Dimensions"
description: "Returns the dimension of a terminal. A terminal is an input terminal or an output terminal of a VI."
---

# ITerminal.Dimensions

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Dimensions fo Terminal

Returns the dimension of a terminal. A terminal is an input terminal or an output terminal of a VI.

## Signature

```python
obj.Dimensions
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem does not support more than two dimensions in the LVRuntime.</td></tr></table>
</div>

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.loadvi(dd.AutoActPath + "Test")

oMyTerminals = objVI.Terminals #Get Terminals
strOutput = "List of terminals:"
for oMyTerminal in oMyTerminals:
    strOutput = strOutput + "\r\n" + "Name: " + oMyterminal.Name()
    strOutput = strOutput + ": Dimension is: " + dd.Str(oMyterminal.Dimensions())
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

*Source: `LVHelper/properties/LVHelper_property_Dimensions_ITerminal.htm`*

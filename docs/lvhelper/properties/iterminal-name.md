---
title: "ITerminal.Name"
description: "Returns the name of an incoming and outgoing VI terminal."
---

# ITerminal.Name

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Name for Terminal

Returns the name of an incoming and outgoing VI terminal.

## Signature

```python
obj.Name
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  You can omit the <span class="Monospace">Name</span> property because the property is a standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test.vi")
oMyTerminals = objVI.Terminals #Get TerminalsDim strOutput
strOutput = "List of terminals:"
for oMyTerminal in oMyTerminals:
    strOutput = strOutput + "\r\n" + "Name: " + oMyterminal.Name
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

*Source: `LVHelper/properties/LVHelper_property_Name_ITerminal.htm`*

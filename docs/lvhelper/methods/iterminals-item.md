---
title: "ITerminals.Item"
description: "Returns the Terminal object for a specific index of a VI. A terminal is an input terminal or an output terminal of a VI."
---

# ITerminals.Item

!!! abstract "Method &middot; `LVHelper.chm`"
    Method: Item for Terminals

Returns the Terminal object for a specific index of a VI. A terminal is an input terminal or an output terminal of a VI.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td>
<td><strong>Note</strong>  You can omit the <span class="Monospace">Item</span> method because it is always the standard element of the collection.</td>
</tr>
</table>
</div>

## Python example

```python
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVi(dd.AutoActPath + "Test")

oMyTerminals = objVI.Terminals #Get Terminals
strOutput = "List of terminals:"
for I in range( 0, oMyTerminals.count-1+1):
    strOutput = strOutput + "\r\n" + "Name: " + oMyterminals.Item(I).Name
dd.MsgBoxDisp(strOutput)

# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
strOutput = strOutput + "\r\n" + "Name: " + oMyterminals(I).Name
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `LVHelper/methods/LVHelper_method_Item_ITerminals.htm`*

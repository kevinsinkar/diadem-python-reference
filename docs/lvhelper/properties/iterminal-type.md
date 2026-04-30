---
title: "ITerminal.Type"
description: "Returns the type of an incoming and outgoing VI terminal."
---

# ITerminal.Type

!!! abstract "Property &middot; `LVHelper.chm`"
    Property: Type for Terminal

Returns the type of an incoming and outgoing VI terminal.

## Signature

```python
obj.Type
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
    strOutput = strOutput + ": Type is: " + oMyterminal.Type()
dd.MsgBoxDisp (strOutput)
# Clean up
objVI = None
dd.LVRuntime.DeInit()
```

```python
# Initialize the LVRuntime
sgRunTimeVersionT = ""
dd.LVRuntime.Init(sgRunTimeVersionT)
# Load "Test.VI"
objVI = dd.LVRuntime.LoadVI(dd.AutoActPath + "Test1.vi")
oMyTerminals = objVI.Terminals #Get Terminals
# Get more details about the terminals
strOutput  = ""
for oMyTerminal  in oMyTerminals:
    strOutput  =  strOutput  + "--------------------------------------------------------------------------" + "\r\n"
    aClusterInfoT = oMyTerminal.Type
    if isinstance(aClusterInfoT, tuple) :
        strOutput  =  strOutput  + "\r\n" + "Name: " + aClusterInfoT(0)
        strOutput  =  strOutput  + "\r\n" + "Type of Clusters: " + aClusterInfoT(1)
        strOutput  =  strOutput  + "\r\n" + "Dimension: " + aClusterInfoT(2)
        strOutput  =  strOutput  + "\r\n" + "Name of first Cluster element: " + aClusterInfoT(3)
        strOutput  =  strOutput  + "\r\n" + "Typ of first Cluster element: " + aClusterInfoT(4)
        strOutput  =  strOutput  + "\r\n" + "Dimension of first Cluster element: " + aClusterInfoT(5)
        strOutput  =  strOutput  + "\r\n" + "Name of second Cluster element: " + aClusterInfoT(6)
    else:
        strOutput  =  strOutput  + "\r\n" + "Name: " + oMyTerminal.Name
        strOutput  =  strOutput  + "\r\n" + "not a Cluster: "

    strOutput  =  strOutput  + "\r\n"

dd.MsgBoxDisp (strOutput)

# Clean upSet TerminalsT = Nothing
dd.VIT = None
dd.LVRuntime.DeInit()
```

---

*Source: `LVHelper/properties/LVHelper_property_Type_ITerminal.htm`*

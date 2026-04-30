---
title: "ITDMContextParameters.Count"
description: "Specifies the number of context parameters in a ContextParameters collection."
---

# ITDMContextParameters.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for ContextParameters

Specifies the number of context parameters in a ContextParameters collection.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("MyASAMServer")
#Generating parameter set
oMyParameterSet = dd.Navigator.Settings.CreateContextParameterSet()
oMyParameterSet.Name = "MyParameterSet"
#Generating parameters and writing parameters into parameter set
oMyParameters = oMyParameterSet.Parameters
oMyParameters.Add("DoubleParameter",1.2345,dd.DataTypeFloat64)
oMyParameters.Add("StringParameter","Parameter",dd.DataTypeString)
#Displaying number of parameters
dd.MsgBoxDisp(oMyParameters.count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMContextParameters.htm`*

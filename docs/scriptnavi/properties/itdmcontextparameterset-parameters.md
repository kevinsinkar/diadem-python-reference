---
title: "ITDMContextParameterSet.Parameters"
description: "Specifies the collection of context parameters in a context parameter set."
---

# ITDMContextParameterSet.Parameters

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Parameters for ContextParameterSet

Specifies the collection of context parameters in a context parameter set.

## Signature

```python
return_value = obj.Parameters
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("Herkules")
#Generating parameter set
oMyParameterSet = dd.Navigator.Settings.CreateContextParameterSet()
oMyParameterSet.Name = "MyParameterSet"
#Generating parameters and writing parameters into parameter set
oMyParameters = oMyParameterSet.Parameters
oMyParameters.Add("DoubleParameter",1.2345,dd.DataTypeFloat64)
oMyParameters.Add("StringParameter","Parameter",dd.DataTypeString)
#Displaying number of parameters
dd.MsgBoxDisp(oMyParameterSet.Parameters.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Parameters_ITDMContextParameterSet.htm`*

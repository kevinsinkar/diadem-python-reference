---
title: "ITDMContextParameters.RemoveAll"
description: "Deletes all context parameters from the collection of context parameters."
---

# ITDMContextParameters.RemoveAll

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: RemoveAll for ContextParameters

Deletes all context parameters from the collection of context parameters.

## Signature

```python
obj.RemoveAll()
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
#Reading all parameters from parameter set
for MyParameter in oMyParameterSet.Parameters:
    dd.MsgBoxDisp("Name: " + MyParameter.Name + "\r\n" + "Value: " + MyParameter.Value + "\r\n" + "Data type: " + MyParameter.DataType)
#Saving, removing and loading parameter set
dd.Navigator.Settings.SaveContextParameterSet("d:\\MyParameterSet.tdp",oMyParameterSet)
oMyParameterSet.Parameters.RemoveAll()
oMyParameterSet = dd.Navigator.Settings.LoadContextParameterSet("d:\\MyParameterSet.tdp")
#Writing parameter set to server
oContext = oMyDataStore.GetContext()
oContext.SetParameters(oMyParameterSet)
#Writing another single parameter to server
oContext.SetParameter("AnotherParam","ParamValue",dd.DataTypeString)
#Reading single parameter from server
MyValue = oContext.GetParameter("AnotherParam")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_RemoveAll_ITDMContextParameters.htm`*

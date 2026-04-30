---
title: "ITDMContextParameter"
description: "The Context Parameter object provides a context parameter. Use the Context . GetParameter method to read context parameters from an ASAM server. Use the Context"
---

# ITDMContextParameter

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ContextParameter

The Context Parameter object provides a context parameter. Use the Context . GetParameter method to read context parameters from an ASAM server. Use the Context . SetParameter method to write context parameters to an ASAM server. Use the Context . SetParameters method to write all context parameters of a Parameter set to an ASAM server.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmcontextparameter-datatype/">DataType</a> | <a href="../../properties/itdmcontextparameter-name/">Name</a> | <a href="../../properties/itdmcontextparameter-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/contextparameters/">ContextParameters</a>.<a href="../../methods/itdmcontextparameters-add/">Add</a> | <a href="../../collections/contextparameters/">ContextParameters</a>.<a href="../../methods/itdmcontextparameters-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMContextParameter.htm`*

---
title: "ITDMContextParameters.Exists"
description: "Checks, whether the context parameter with the specified name already exists."
---

# ITDMContextParameters.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for ContextParameters

Checks, whether the context parameter with the specified name already exists.

## Signature

```python
bExists = Object.Exists(Name)
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
#Checking if parameter exists
dd.MsgBoxDisp(oMyParameters.Exists("StringParameter"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ITDMContextParameters.htm`*

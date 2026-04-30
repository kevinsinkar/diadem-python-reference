---
title: "ITDMContextParameters.Remove"
description: "Deletes a context parameter from the collection of context parameters."
---

# ITDMContextParameters.Remove

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Remove for ContextParameters

Deletes a context parameter from the collection of context parameters.

## Signature

```python
obj.Remove(NameOrIndex)
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
#Deleting second parameter
oMyParameters.Remove(2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Remove_ITDMContextParameters.htm`*

---
title: "ITDMContextParameters.Item"
description: "Returns the ContextParameter object associated with a specific name or with a specific index."
---

# ITDMContextParameters.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for ContextParameters

Returns the ContextParameter object associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(NameOrIndex)
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
#Displaying second parameter name
dd.MsgBoxDisp(oMyParameters.Item(2).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_ITDMContextParameters.htm`*

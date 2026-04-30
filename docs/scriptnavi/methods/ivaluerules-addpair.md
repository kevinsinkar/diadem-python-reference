---
title: "IValueRules.AddPair"
description: "Adds a new mapping pair for a simple 1:1 replacement, when mapping values of a property."
---

# IValueRules.AddPair

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: AddPair for ValueMappingRules

Adds a new mapping pair for a simple 1:1 replacement, when mapping values of a property.

## Signature

```python
return_value = obj.AddPair(OriginalString, OutputString)
```

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyPair = oMyChnNameMapping.Rules.AddPair("Example_1", "Example~1")
dd.MsgBoxDisp("Pair: " + oMyPair.Pattern + " => " + oMyPair.Schema) #Pair => Example_1 => Example~1
```

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([[:alpha:]]+)([\\_\\-\\/\\\\?\\ \\:]+)([[:digit:]]+)","$1~text~$3","Example_1")
print ("Pattern: " , oMyRule.Pattern , "\r\n" , "Scheme: " , oMyRule.Schema , "\r\n" , "Example to map: " , oMyRule.Example , "\r\n" , "Mapped example: " , oMyRule.MapProperty(oMyRule.Example)) #Mapped example =>  Example~text~1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_AddPair_IValueRules.htm`*

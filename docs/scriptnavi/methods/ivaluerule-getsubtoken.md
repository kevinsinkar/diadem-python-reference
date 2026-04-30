---
title: "IValueRule.GetSubToken"
description: "Returns the sections of an input text defined by Search pattern and Replacement pattern , when mapping values of a property. If the value of a property is, for "
---

# IValueRule.GetSubToken

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetSubToken for ValueRule

Returns the sections of an input text defined by Search pattern and Replacement pattern , when mapping values of a property. If the value of a property is, for example, Example_1 , the first token is the text Example , the second token is the underscore, and the third token is the digit 1 .

## Signature

```python
obj.GetSubToken(InputText, pValues, pPattern)
```

## Python example

```python
ValueArray   = Array
PatternArray = Array

oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyRule = oMyChnNameMapping.Rules.Add("([A-Za-z]+)([\\_\\-\\/\\\\?\\ \\:]+)([0-9]+)","$1$3","Example_1")
oMyRule.GetSubToken("Example_1", ValueArray, PatternArray)
sTxt = ""
for I in range( 0, len(ValueArray)-1):
    sTxt = sTxt + "SubToken("+I+")    Value: "+ ValueArray(I) + string(10," ") + "Pattern: " + PatternArray(I) + "\r\n"
print (sTxt)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetSubToken_IValueRule.htm`*

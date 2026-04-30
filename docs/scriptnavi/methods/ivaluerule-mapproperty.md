---
title: "IValueRule.MapProperty"
description: "Applies the rule specified in the ValueRule object to the transferred text when mapping rules, in order to replace values of properties. Note Use the MapPropert"
---

# IValueRule.MapProperty

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: MapProperty for ValueRule

Applies the rule specified in the ValueRule object to the transferred text when mapping rules, in order to replace values of properties. Note Use the MapProperty for PropertyValueMapping method in order to apply all defined rules to the transferred text, when mapping values.

## Signature

```python
sMapProperty = Object.MapProperty(InputText)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../ivaluemapping-mapproperty/">MapProperty for PropertyValueMapping</a> method in order to apply all defined rules to the transferred text, when mapping values.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If a search pattern cannot be used completely on a transferred text, DIAdem returns an empty string.</td></tr></table>
</div>

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyPair = oMyChnNameMapping.Rules.AddPair("Example_1", "Example~1")
dd.MsgBoxDisp ("Mapped Example: " + oMyPair.MapProperty("Example_1")) #Mapped Example => Example~1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_MapProperty_IValueRule.htm`*

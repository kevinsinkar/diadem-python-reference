---
title: "IValueMapping.MapProperty"
description: "Applies all rules of the PropertyValueMapping collection to the passed text when mapping values. DIAdem applies all mapping rules in the defined order and retur"
---

# IValueMapping.MapProperty

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: MapProperty for PropertyValueMapping

Applies all rules of the PropertyValueMapping collection to the passed text when mapping values. DIAdem applies all mapping rules in the defined order and returns the replacement text. Note Use the MapProperty for ValueRule method in order to apply only one rule to the transferred text when mapping rules.

## Signature

```python
sMapProperty = Object.MapProperty(InputText)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use the <a href="../ivaluerule-mapproperty/">MapProperty for ValueRule</a> method in order to apply only one rule to the transferred text when mapping rules.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If a search pattern cannot be used on a transferred text, DIAdem returns an empty string.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note </strong> In rules with search pattern rules, all rules from 1 to n are executed. The mapping result corresponds with the first rule that can be applied without errors.</td></tr></table>
</div>

## Python example

```python
oMyMapper = dd.Navigator.Settings.CreateValueMapper()
oMyChnNameMapping = oMyMapper.Mappings(dd.eSearchChannel).Add("name")
oMyPair1 = oMyChnNameMapping.Rules.AddPair("Example_1", "Example~1")
oMyPair2 = oMyChnNameMapping.Rules.AddPair("Example-2", "Example~2")
dd.MsgBoxDisp ("Mapped Example: " + oMyChnNameMapping.MapProperty("Example_1")) #Mapped Example => Example~1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_MapProperty_IValueMapping.htm`*

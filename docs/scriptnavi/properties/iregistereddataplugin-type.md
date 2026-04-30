---
title: "IRegisteredDataPlugin.Type"
description: "Specifies the type of a DataPlugin registered on your computer."
---

# IRegisteredDataPlugin.Type

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Type for RegisteredDataPlugin <Navigator>

Specifies the type of a DataPlugin registered on your computer.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePluginCodeUnknown` | 42110 | Unknown |
| `ePluginCodeVbs` | 42111 | VBS |
| `ePluginCodeVbCrypt` | 42112 | VBCrypt |
| `ePluginCodeC` | 42113 | C |
| `ePluginCodeLabVIEW` | 42114 | LabVIEW |
| `ePluginCodePython` | 42115 | Python |
| `ePluginCodePyCrypt` | 42116 | Python Crypt |

## Python example

```python
def TypeofDataPlugin(sType):
    select_variable_0 = sType
    if (select_variable_0 == dd.ePluginCodeUnknown) :
        TypeofDataPlugin = "Unknown"
    elif (select_variable_0 == dd.ePluginCodeVbs) :
        TypeofDataPlugin = "VBS"
    elif (select_variable_0 == dd.ePluginCodeVbCrypt) :
        TypeofDataPlugin = "VBCrypt"
    elif (select_variable_0 == dd.ePluginCodeC) :
        TypeofDataPlugin = "C"
    elif (select_variable_0 == dd.ePluginCodeLabVIEW) :
        TypeofDataPlugin = "LabVIEW"
    elif (select_variable_0 == dd.ePluginCodePython) :
        TypeofDataPlugin = "Python"
    elif (select_variable_0 == dd.ePluginCodePyCrypt) :
        TypeofDataPlugin = "Python-Crypt"
    return TypeofDataPlugin

sMyDataPluginName = "GPX"
oMyDataPlugin = dd.Navigator.Settings.RegisteredDataPlugins(sMyDataPluginName)
print(TypeofDataPlugin(oMyDataPlugin.Type))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Type_IRegisteredDataPlugin.htm`*

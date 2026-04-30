---
title: "IUpdateDataDataPlugin.Type"
description: "Specifies the DataPlugin type."
---

# IUpdateDataDataPlugin.Type

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Type for UpdateDataDataPlugin <Navigator>

Specifies the DataPlugin type.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePluginCodeUnknown` | 42110 | Unknown type |
| `ePluginCodeVbs` | 42111 | VBS |
| `ePluginCodeVbCrypt` | 42112 | VBCrypt |
| `ePluginCodeC` | 42113 | C |
| `ePluginCodeLabVIEW` | 42114 | LabVIEW |
| `ePluginCodePython` | 42115 | Python |
| `ePluginCodePyCrypt` | 42116 | Python encrypted |

## Python example

```python
def UpdateData2Text(sType):
    select_variable_0 = sType
    if (select_variable_0 == dd.ePluginCodeUnknown) :
        UpdateData2Text = "Unknown"
    elif (select_variable_0 == dd.ePluginCodeVbs) :
        UpdateData2Text = "VBS"
    elif (select_variable_0 == dd.ePluginCodeVbCrypt) :
        UpdateData2Text = "VBCrypt"
    elif (select_variable_0 == dd.ePluginCodeC) :
        UpdateData2Text = "C"
    elif (select_variable_0 == dd.ePluginCodeLabVIEW) :
        UpdateData2Text = "LabVIEW"
    return UpdateData2Text

oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
dd.MsgBoxDisp(UpdateData2Text(oMyDataUpdateSource.UpdateData("GPX").Type))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Type_IUpdateDataDataPlugin.htm`*

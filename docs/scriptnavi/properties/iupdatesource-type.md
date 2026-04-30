---
title: "IUpdateSource.Type"
description: "Specifies with which update source you synchronize your local DataPlugins."
---

# IUpdateSource.Type

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Type for UpdateSource <Navigator>

Specifies with which update source you synchronize your local DataPlugins.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eUpdateSourceNiWeb` | 42001 | The NI DataPlugin website is the update source. |
| `eUpdateSourceNiDFSE` | 42002 | The specified DataFinder instance is the update source. |

## Python example

```python
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource(dd.eUpdateSourceNiWeb)
dd.MsgBoxDisp("Type: " + oMyDataUpdateSource.Type + "\r\n" + "Last Update: " + oMyDataUpdateSource.LastUpdate)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Type_IUpdateSource.htm`*

---
title: "IUpdateSource.CompareVersion"
description: "Compares the local version of a VBS DataPlugin with the version of the same DataPlugin in the update source."
---

# IUpdateSource.CompareVersion

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CompareVersion for UpdateSource <Navigator>

Compares the local version of a VBS DataPlugin with the version of the same DataPlugin in the update source.

## Signature

```python
eCompareVersion = Object.CompareVersion(DataPluginName)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eCompNoVersion` | 42100 | No version information available. |
| `eCompSameVersion` | 42101 | The local version and the version in the update source are the same. |
| `eCompLowerVersion` | 42102 | The version in the update source is lower than the local version. |
| `eCompHigherVersion` | 42103 | The version in the update source is higher than the local version. |
| `eCompUnknownVersion` | 42104 | Unknown version. A comparison is not possible. |

## Python example

```python
def CompareDPVersion(sCompare):
    select_variable_0 = sCompare
    if (select_variable_0 == dd.eCompNoVersion) :
        CompareDPVersion = "No version information"
    elif (select_variable_0 == dd.eCompSameVersion) :
        CompareDPVersion = "Same version"
    elif (select_variable_0 == dd.eCompLowerVersion) :
        CompareDPVersion = "Local version is higher"
    elif (select_variable_0 == dd.eCompHigherVersion) :
        CompareDPVersion = "Local version is lower"
    elif (select_variable_0 == dd.eCompUnknownVersion) :
        CompareDPVersion = "Unknown version"
    return CompareDPVersion

oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
dd.MsgBoxDisp(CompareDPVersion(oMyDataUpdateSource.CompareVersion("GPX")))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_CompareVersion_IUpdateSource.htm`*

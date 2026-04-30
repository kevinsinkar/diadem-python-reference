---
title: "ITDMResultsDisplaySettings.ColumnHeaderDisplayMode"
description: "Specifies whether DIAdem displays the names of the layers and the associated properties in the column header of the search result list or whether DIAdem hides t"
---

# ITDMResultsDisplaySettings.ColumnHeaderDisplayMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ColumnHeaderDisplayMode for ResultsListSettings

Specifies whether DIAdem displays the names of the layers and the associated properties in the column header of the search result list or whether DIAdem hides the layers and only displays the properties.

## Signature

```python
obj.ColumnHeaderDisplayMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eResultsHdrModeLevelProperty` | 1 | DIAdem displays the names of the layers and the names of the properties in the column header of the search results list (default value). |
| `eResultsHdrModeProperty` | 2 | DIAdem hides in the column header of the search results list the names of the layers and displays only the names of the properties. |

## Python example

```python
oMyReportObj = dd.Navigator.Display.CurrDataFinder.ResultsList.Settings
oMyReportObj.ColumnHeaderDisplayMode = dd.eResultsHdrModeProperty
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ColumnHeaderDisplayMode_ITDMResultsDisplaySettings.htm`*

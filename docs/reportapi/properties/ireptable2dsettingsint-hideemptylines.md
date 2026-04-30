---
title: "IRepTable2DSettingsInt.HideEmptyLines"
description: "Specifies whether DIAdem hides the rows in which the values of all columns contain the value NoValue or an empty string. DIAdem only includes the propertyif you"
---

# IRepTable2DSettingsInt.HideEmptyLines

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: HideEmptyLines for 2DTableSettings

Specifies whether DIAdem hides the rows in which the values of all columns contain the value NoValue or an empty string. DIAdem only includes the propertyif you selected the value e2DTableIndexModeAutomaticallyIncreasing for the IndexMode property.

## Signature

```python
obj.HideEmptyLines
```

## Python example

```python
o2DTable = dd.Report.ActiveSheet.Objects("2DTable1")
o2DTable.Settings.HideEmptyLines = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_HideEmptyLines_IRepTable2DSettingsInt.htm`*

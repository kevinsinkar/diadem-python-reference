---
title: "IRepExpansionLineStyleListInt.Count"
description: "Changes the number of settings which DIAdem uses for curve display in REPORT layouts with Curve expansion or returns this value."
---

# IRepExpansionLineStyleListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for ExpansionLineStyles

Changes the number of settings which DIAdem uses for curve display in REPORT layouts with Curve expansion or returns this value.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReportObj = dd.Report.Settings.CurveExpansion.AttributeList.LineStyles
dd.MsgBoxDisp("Number of expansion line definitions: " + oMyReportObj.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepExpansionLineStyleListInt.htm`*

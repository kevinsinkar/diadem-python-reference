---
title: "IRepExpansionLineStyleListInt.Add"
description: "Adds settings which DIAdem uses to display REPORT layouts with Curve expansion ."
---

# IRepExpansionLineStyleListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for ExpansionLineStyles

Adds settings which DIAdem uses to display REPORT layouts with Curve expansion .

## Signature

```python
return_value = obj.Add()
```

## Python example

```python
dd.Report.NewLayout()
oMyReportSettings = dd.Report.Settings
oMyCurveExpansion = oMyReportSettings.CurveExpansion
oMyCurveExpansion.Enable = True
oMyAttributeList = oMyCurveExpansion.AttributeList
oMyAttributeList.Enable = True
oMyExpansionLineStyle = oMyAttributeList.LineStyles
oMyAttributeList.UseLineInterval = True
oMyAttributeList.UseLineType = True
oMyAttributeList.UseLineWidth = True
oMyAttributeList.UseMarkerProperties = True
oMyAttributeList.UseMarkerType = True

dd.MsgBoxDisp("No: " + oMyExpansionLineStyle.Count)
oMyExpansionLineStyle.Add()
I = oMyExpansionLineStyle.Count
dd.MsgBoxDisp("No: " + oMyExpansionLineStyle.Count)
oMyExpansionLineStyle(I).Line.Width = dd.eLineWidth0070
oMyExpansionLineStyle(I).Line.LineType = dd.eLineTypeDashDot
oMyExpansionLineStyle(I).Line.Interval = 5
oMyExpansionLineStyle(I).Marker.Size = 3
oMyExpansionLineStyle(I).Marker.Type = dd.eMarkerCircle
oMyExpansionLineStyle(I).Marker.RepetitionMode = dd.eMarkerRepetitionMaximalNPoints
oMyExpansionLineStyle(I).Marker.MarkerPointCount = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepExpansionLineStyleListInt.htm`*

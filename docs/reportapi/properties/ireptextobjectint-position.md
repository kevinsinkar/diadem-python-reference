---
title: "IRepTextObjectInt.Position"
description: "Specifies the position of a Text object in a DIAdem REPORT worksheet."
---

# IRepTextObjectInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for RTFText

Specifies the position of a Text object in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMyRTFText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectRTFText,"MyRtfText")
oMyRTFTextPosition = oMyRTFText.Position
oMyRTFTextPosition.ByCoordinate.X1 = 100
oMyRTFTextPosition.ByCoordinate.X2 = 30
oMyRTFTextPosition.ByCoordinate.Y1 = 50
oMyRTFTextPosition.ByCoordinate.Y2 = 10
dd.Report.Refresh()
oMyRTFText.ExportToImage("MyRtfText",dd.eImageExportTypePNG)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepTextObjectInt.htm`*

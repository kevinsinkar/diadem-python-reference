---
title: "IRepFrameLineInt.LineType"
description: "Specifies the line type of a frame in DIAdem REPORT."
---

# IRepFrameLineInt.LineType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineType for FrameLine

Specifies the line type of a frame in DIAdem REPORT.

## Signature

```python
obj.LineType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineTypeNone` | 0 | None |
| `eLineTypeSolid` | 1 | Line |
| `eLineTypeDashDot` | 2 | Dots and dashes |
| `eLineTypeDashed1` | 3 | Dashes 1 |
| `eLineTypeDashed2` | 4 | Dashes 2 |
| `eLineTypeDotted` | 5 | Dotted |

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.BorderLine.LineType = dd.eLineTypeDotted
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LineType_IRepFrameLineInt.htm`*

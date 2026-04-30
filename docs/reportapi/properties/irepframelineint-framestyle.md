---
title: "IRepFrameLineInt.FrameStyle"
description: "Specifies whether the frame of a comment lies within the edge or is centered on the edge."
---

# IRepFrameLineInt.FrameStyle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FrameStyle for FrameLine

Specifies whether the frame of a comment lies within the edge or is centered on the edge.

## Signature

```python
obj.FrameStyle
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eFrameStyleInwards` | 0 | Frame within the comment frame |
| `eFrameStyleCentric` | 1 | Frame centered on the comment frame |

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyFrameLine = oMyComment.Comment.BorderLine
oMyFrameLine.UseIndividualLineStyle  = False
oMyFrameLine.FrameStyle = dd.eFrameStyleCentric
oMyFrameLine.LineType = dd.eLineTypeDotted
oMyFrameLine.Width = dd.eLineWidth0140
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FrameStyle_IRepFrameLineInt.htm`*

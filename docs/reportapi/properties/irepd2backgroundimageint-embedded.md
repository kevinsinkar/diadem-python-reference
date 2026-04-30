---
title: "IRepD2BackgroundImageInt.Embedded"
description: "Specifies whether DIAdem REPORT embeds the background graphic of a 2D axis system in the layout file."
---

# IRepD2BackgroundImageInt.Embedded

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Embedded for 2DBackgroundImage

Specifies whether DIAdem REPORT embeds the background graphic of a 2D axis system in the layout file.

## Signature

```python
obj.Embedded
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySetting = oMy2DAxisSystem.Settings
oMyBackgroundImage = oMySetting.BackgroundImage
oMyBackgroundImage.FileName = "Example1.png"
oMyBackgroundImage.Scaling.Enable = True
oMyBackgroundImage.Scaling.XBegin = 10
oMyBackgroundImage.Scaling.XEnd = 40
oMyBackgroundImage.Scaling.YBegin = 20
oMyBackgroundImage.Scaling.YEnd = 50
oMyBackgroundImage.Embedded = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Embedded_IRepD2BackgroundImageInt.htm`*

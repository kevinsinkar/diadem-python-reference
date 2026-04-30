---
title: "IRepD2BackgroundImageInt"
description: "The 2DBackgroundImage object provides the properties of a background graphic in a 2D axis system in DIAdem REPORT."
---

# IRepD2BackgroundImageInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBackgroundImage

The 2DBackgroundImage object provides the properties of a background graphic in a 2D axis system in DIAdem REPORT.

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
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2backgroundimageint-embedded/">Embedded</a> | <a href="../../properties/irepd2backgroundimageint-filename/">FileName</a> | <a href="../../properties/irepd2backgroundimageint-fullpath/">FullPath</a> | <a href="../../properties/irepd2backgroundimageint-scaling/">Scaling</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axissettingsint/">2DAxisSettings</a>.<a href="../../properties/irepd2axissettingsint-backgroundimage/">BackgroundImage</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2BackgroundImageInt.htm`*

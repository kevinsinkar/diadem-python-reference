---
title: "IRepD2BackgroundImageInt.FullPath"
description: "Specifies the complete path and the filename of the background graphic in a 2D axis system in DIAdem REPORT."
---

# IRepD2BackgroundImageInt.FullPath

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FullPath for 2DBackgroundImage

Specifies the complete path and the filename of the background graphic in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.FullPath
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
oMyBackgroundImage.Scaling.XEnd = 50
oMyBackgroundImage.Scaling.YBegin = 20
oMyBackgroundImage.Scaling.YEnd = 40
dd.MsgBoxDisp(oMyBackgroundImage.FullPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FullPath_IRepD2BackgroundImageInt.htm`*

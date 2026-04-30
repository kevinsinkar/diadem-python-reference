---
title: "IRepD2AxisSettingsInt"
description: "The 2DAxisSettings object provides the properties of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DAxisSettings

The 2DAxisSettings object provides the properties of a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy2DAxisSystem.Settings
oMySettings.Grid.DisplayMode = dd.e2DAxisGridModeGrid
oMySettings.Grid.MiniTickGrid.Visible = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2axissettingsint-axisline/">AxisLine</a> | <a href="../../properties/irepd2axissettingsint-axisscalemode/">AxisScaleMode</a> | <a href="../../properties/irepd2axissettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepd2axissettingsint-backgroundimage/">BackgroundImage</a> | <a href="../../properties/irepd2axissettingsint-backgroundsegments/">BackgroundSegments</a> | <a href="../../properties/irepd2axissettingsint-grid/">Grid</a> | <a href="../../properties/irepd2axissettingsint-nsystemsmode/">NSystemsMode</a> | <a href="../../properties/irepd2axissettingsint-usecommonxchannel/">UseCommonXChannel</a> | <a href="../../properties/irepd2axissettingsint-usecurvetransformation/">UseCurveTransformation</a> | <a href="../../properties/irepd2axissettingsint-useindividualaxisstyle/">UseIndividualAxisStyle</a> | <a href="../../properties/irepd2axissettingsint-useisometricratio/">UseIsometricRatio</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2AxisSettingsInt.htm`*

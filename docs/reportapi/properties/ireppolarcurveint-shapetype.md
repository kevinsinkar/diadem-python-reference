---
title: "IRepPolarCurveInt.ShapeType"
description: "Specifies the display mode of a curve in a polar axis system in DIAdem REPORT. You can use the ChangeShape for PolarCurves method to change the display mode."
---

# IRepPolarCurveInt.ShapeType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShapeType for PolarCurve

Specifies the display mode of a curve in a polar axis system in DIAdem REPORT. You can use the ChangeShape for PolarCurves method to change the display mode.

## Signature

```python
obj.ShapeType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarShapeLine` | 0 | Line |
| `ePolarShapeLineAndPoints` | 1 | Line and points |
| `ePolarShapeSpikes` | 2 | Spikes |
| `ePolarShapeDifferential` | 3 | Differential |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarSystem")
oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyPolarCurve.Shape.YChannel.Reference = "[5]/[2]"
dd.MsgBoxDisp(oMyPolarCurve.ShapeType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShapeType_IRepPolarCurveInt.htm`*

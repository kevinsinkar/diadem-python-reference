---
title: "IRepSpiderSelectedSubObjectsListInt.AddSpider"
description: "Selects the subobject of a spider axis system in DIAdem REPORT associated with a specific index."
---

# IRepSpiderSelectedSubObjectsListInt.AddSpider

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: AddSpider for SpiderSelectedElements

Selects the subobject of a spider axis system in DIAdem REPORT associated with a specific index.

## Signature

```python
return_value = obj.AddSpider(ElementType, Index)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderElementAxis` | 0 | Axis |
| `eSpiderElementAxisNumbers` | 1 | Axis scale |
| `eSpiderElementAxisLabel` | 2 | Show/hide |
| `eSpiderElementCurve` | 3 | Curve |
| `eSpiderElementCurveLegend` | 4 | Legend |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider,"MySpiderSystem")
oMyPosition = oMyAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MyNewCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"
dd.Report.Refresh()
oMyAxisSystem.SelectedElements.AddSpider(dd.eSpiderElementAxis, 1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_AddSpider_IRepSpiderSelectedSubObjectsListInt.htm`*

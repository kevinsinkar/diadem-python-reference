---
title: "IRepBaseCtrlInt"
description: "The ReportObject object provides an object for graphical display in DIAdem REPORT. The ReportObject object corresponds to one of the following objects: 2DAxisSy"
---

# IRepBaseCtrlInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ReportObject

The ReportObject object provides an object for graphical display in DIAdem REPORT. The ReportObject object corresponds to one of the following objects: 2DAxisSystem (IRepD2AxisInt) 2D axis system 2DTable (IRepTable2DInt) 2D Table 3DAxisSystem (IRepD3AxisInt) 3D axis system 3DTable (IRepTable3DInt) 3D table Arrow (IRepArrowInt) Line and arrow Circle (IRepCircleInt) Circle Comment (IRepCommentInt) Comment FormulaDisplay (IRepFormulaDisplayInt) Formula graphic Frame (IRepFreeFrameInt) Free frame Image (IRepImageInt) Any graphic PieChart (IRepPieChartInt) Pie chart PolarSystem (IRepPolarInt) 2D polar axis system RTFText (IRepTextObjectInt) Text object Spider (IRepSpiderInt) Spider axis system Text (IRepTextSimpleInt) Free text

## Python example

```python
sOutput = ""
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    sOutput = sOutput + "Object type: " + oMyReportObj.ObjectType + "\t" + "Object name: " + oMyReportObj.Name + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepbasectrlint-index/">Index</a> | <a href="../../properties/irepbasectrlint-isselected/">IsSelected</a> | <a href="../../properties/irepbasectrlint-name/">Name</a> | <a href="../../properties/irepbasectrlint-objecttype/">ObjectType</a> | <a href="../../properties/irepbasectrlint-tagstored/">TagStored</a> | <a href="../../properties/irepbasectrlint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepbasectrlint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepbasectrlint-select/">Select</a> | <a href="../../methods/irepbasectrlint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepBaseCtrlInt.htm`*

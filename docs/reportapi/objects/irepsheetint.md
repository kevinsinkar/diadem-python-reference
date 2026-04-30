---
title: "IRepSheetInt"
description: "The Sheet object provides a worksheet in DIAdem REPORT."
---

# IRepSheetInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Sheet

The Sheet object provides a worksheet in DIAdem REPORT.

## Python example

```python
for oMySheet in dd.Report.Sheets:
    dd.MsgBoxDisp(oMySheet.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepsheetint-dimensions/">Dimensions</a> | <a href="../../properties/irepsheetint-events/">Events</a> | <a href="../../properties/irepsheetint-index/">Index</a> | <a href="../../properties/irepsheetint-name/">Name</a> | <a href="../../properties/irepsheetint-objects/">Objects</a> | <a href="../../properties/irepsheetint-subsheets/">SubSheets</a> | <a href="../../properties/irepsheetint-tagstored/">TagStored</a> | <a href="../../properties/irepsheetint-tagtemporary/">TagTemporary</a> | <a href="../../properties/irepsheetint-useforprinting/">UseForPrinting</a> | <a href="../../properties/irepsheetint-usemasterlayout/">UseMasterLayout</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepsheetint-activate/">Activate</a> | <a href="../../methods/irepsheetint-exporttoclipboard/">ExportToClipboard</a> | <a href="../../methods/irepsheetint-exporttoimage/">ExportToImage</a> | <a href="../../methods/irepsheetint-exporttopdf/">ExportToPDF</a> | <a href="../../methods/irepsheetint-exporttopdfmsprint/">ExportToPDFMSPrint</a> | <a href="../../methods/irepsheetint-exporttopdfmsprint/">ExportToXPS</a> | <a href="../../methods/irepsheetint-exporttoxps/">Print</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptable2dcolumndrawingcontextint/">2DTableColumnDrawingContext</a>.<a href="../../properties/ireptable2dcolumndrawingcontextint-sheet/">Sheet</a> | <a href="../ireptable2ddrawingcellcontextint/">2DTableDrawingCellContext</a>.<a href="../../properties/ireptable2ddrawingcellcontextint-sheet/">Sheet</a> | <a href="../ireptable2ddrawingheaderfootercellcontextint/">2DTableDrawingHeaderFooterCellContext</a>.<a href="../../properties/ireptable2ddrawingheaderfootercellcontextint-sheet/">Sheet</a> | <a href="../ireptable2ddropcontextint/">2DTableDropContext</a>.<a href="../../properties/ireptable2ddropcontextint-sheet/">Sheet</a> | <a href="../ireptable3ddropcontextint/">3DTableDropContext</a>.<a href="../../properties/ireptable3ddropcontextint-sheet/">Sheet</a> | <a href="../irepcommentdropcontextint/">CommentDropContext</a>.<a href="../../properties/irepcommentdropcontextint-sheet/">Sheet</a> | <a href="../irepcustomscalingaxissystem2dcontextint/">CustomScalingAxisSystem2DContext</a>.<a href="../../properties/irepcustomscalingaxissystem2dcontextint-sheet/">Sheet</a> | <a href="../irepcustomscalingaxissystem2dscaledcontextint/">CustomScalingAxisSystem2DScaledContext</a>.<a href="../../properties/irepcustomscalingaxissystem2dscaledcontextint-sheet/">Sheet</a> | <a href="../irepcustomscalingaxissystem3dcontextint/">CustomScalingAxisSystem3DContext</a>.<a href="../../properties/irepcustomscalingaxissystem3dcontextint-sheet/">Sheet</a> | <a href="../irepd2axissystemclickedwithkeycontextint/">D2AxisSystemClickedWithKeyContext</a>.<a href="../../properties/irepd2axissystemclickedwithkeycontextint-sheet/">Sheet</a> | <a href="../irepd2axisdropcontextint/">D2AxisSystemDropContext</a>.<a href="../../properties/irepd2axisdropcontextint-sheet/">Sheet</a> | <a href="../irepd2curvedrawingcontextint/">D2CurveDrawingContext</a>.<a href="../../properties/irepd2curvedrawingcontextint-sheet/">Sheet</a> | <a href="../irepd2curvetransformingcontextint/">D2CurveTransformingContext</a>.<a href="../../properties/irepd2curvetransformingcontextint-sheet/">Sheet</a> | <a href="../irepd3axisdropcontextint/">D3AxisSystemDropContext</a>.<a href="../../properties/irepd3axisdropcontextint-sheet/">Sheet</a> | <a href="../irepd3curvedrawingcontextint/">D3CurveDrawingContext</a>.<a href="../../properties/irepd3curvedrawingcontextint-sheet/">Sheet</a> | <a href="../irepd3curvetransformingcontextint/">D3CurveTransformingContext</a>.<a href="../../properties/irepd3curvetransformingcontextint-sheet/">Sheet</a> | <a href="../ireppagedropcontextint/">PageDropContext</a>.<a href="../../properties/ireppagedropcontextint-sheet/">Sheet</a> | <a href="../ireppolaraxissystemclickedwithkeycontextint/">PolarAxisSystemClickedWithKeyContext</a>.<a href="../../properties/ireppolaraxissystemclickedwithkeycontextint-sheet/">Sheet</a> | <a href="../ireppolarcurvedrawingcontextint/">PolarCurveDrawingContext</a>.<a href="../../properties/ireppolarcurvedrawingcontextint-sheet/">Sheet</a> | <a href="../ireppolardropcontextint/">PolarSystemDropContext</a>.<a href="../../properties/ireppolardropcontextint-sheet/">Sheet</a> | <a href="../irepreportint/">Report</a>.<a href="../../properties/irepreportint-activesheet/">ActiveSheet</a> | <a href="../../collections/sheets/">Sheets</a>.<a href="../../methods/irepsheetlistint-add/">Add</a> | <a href="../../collections/sheets/">Sheets</a>.<a href="../../methods/irepsheetlistint-copy/">Copy</a> | <a href="../../collections/sheets/">Sheets</a>.<a href="../../methods/irepsheetlistint-insert/">Insert</a> | <a href="../../collections/sheets/">Sheets</a>.<a href="../../methods/irepsheetlistint-item/">Item</a> | <a href="../ireptable2dcolumntransformingcontextint/">Table2DColumnTransformingContext</a>.<a href="../../properties/ireptable2dcolumntransformingcontextint-sheet/">Sheet</a> | <a href="../ireptextsimpledropcontextint/">TextDropContext</a>.<a href="../../properties/ireptextsimpledropcontextint-sheet/">Sheet</a> | <a href="../ireptooltip2daxiscontextint/">ToolTip2DAxisContext</a>.<a href="../../properties/ireptooltip2daxiscontextint-sheet/">Sheet</a> | <a href="../ireptooltip2dtablecontextint/">ToolTip2DTableContext</a>.<a href="../../properties/ireptooltip2dtablecontextint-sheet/">Sheet</a> | <a href="../ireptooltip3daxiscontextint/">ToolTip3DAxisContext</a>.<a href="../../properties/ireptooltip3daxiscontextint-sheet/">Sheet</a> | <a href="../ireptooltip3dtablecontextint/">ToolTip3DTableContext</a>.<a href="../../properties/ireptooltip3dtablecontextint-sheet/">Sheet</a> | <a href="../ireptooltiparrowcontextint/">ToolTipArrowContext</a>.<a href="../../properties/ireptooltiparrowcontextint-sheet/">Sheet</a> | <a href="../ireptooltipcirclecontextint/">ToolTipCircleContext</a>.<a href="../../properties/ireptooltipcirclecontextint-sheet/">Sheet</a> | <a href="../ireptooltipcommentcontextint/">ToolTipCommentContext</a>.<a href="../../properties/ireptooltipcommentcontextint-sheet/">Sheet</a> | <a href="../ireptooltipformuladisplaycontextint/">ToolTipFormulaDisplayContext</a>.<a href="../../properties/ireptooltipformuladisplaycontextint-sheet/">Sheet</a> | <a href="../ireptooltipframecontextint/">ToolTipFrameContext</a>.<a href="../../properties/ireptooltipframecontextint-sheet/">Sheet</a> | <a href="../ireptooltipimagecontextint/">ToolTipImageContext</a>.<a href="../../properties/ireptooltipimagecontextint-sheet/">Sheet</a> | <a href="../ireptooltippiechartcontextint/">ToolTipPieChartContext</a>.<a href="../../properties/ireptooltippiechartcontextint-sheet/">Sheet</a> | <a href="../ireptooltippolarcontextint/">ToolTipPolarContext</a>.<a href="../../properties/ireptooltippolarcontextint-sheet/">Sheet</a> | <a href="../ireptooltipspidercontextint/">ToolTipSpiderContext</a>.<a href="../../properties/ireptooltipspidercontextint-sheet/">Sheet</a> | <a href="../ireptooltiptextcontextint/">ToolTipTextContext</a>.<a href="../../properties/ireptooltiptextcontextint-sheet/">Sheet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSheetInt.htm`*

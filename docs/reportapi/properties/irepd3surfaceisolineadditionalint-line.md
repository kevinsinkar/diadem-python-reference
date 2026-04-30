---
title: "IRepD3SurfaceIsolineAdditionalInt.Line"
description: "Specifies the properties of the additional isolines in the Surface display mode in a 3D axis system in DIAdem REPORT."
---

# IRepD3SurfaceIsolineAdditionalInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 3DAdditionalSurfaceIsoline

Specifies the properties of the additional isolines in the Surface display mode in a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem :
        oMyCurves = oMyReportObj.Curves3D
        for oMyCurve in oMyCurves:
            if oMyCurve.ShapeType == dd.e3DShapeSurface :
                oMySurfaceLine = oMyCurve.Shape.Extensions.SurfaceIsoline
                oMySurfaceLine.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected
                oMySurfaceLine.Visible = True
                oMySurfaceLine.Line.Color.SetPredefinedColor(dd.eColorIndexPalette)
                oMyColoredLines = oMyCurve.Shape.Settings.Palette
                for i in range( 1, oMyColoredLines.Count+1):
                    oMyColoredLines(i).LineType = dd.eLineTypeDashDot
                    oMyColoredLines(i).Width = dd.eLineWidth0050
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMyReportObj, oMyReportObjects, oMyCurves, oMyCurve, oMySurfaceLine, oMyColoredLines, i
<span class="HlVBSKeyword">Set</span> oMyReportObjects = <span class="Hldiademobject">Report.ActiveSheet.Objects</span>
<span class="HlVBSKeyword">For</span> <span class="HlVBSKeyword">Each</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects
  <span class="HlVBSKeyword">If</span> oMyReportObj.ObjectType = <span class="Hldiademconstant">eReportObject3DAxisSystem</span> <span class="HlVBSKeyword">Then</span>
    <span class="HlVBSKeyword">Set</span> oMyCurves = oMyReportObj.Curves3D
    <span class="HlVBSKeyword">For</span> <span class="HlVBSKeyword">Each</span> oMyCurve <span class="HlVBSKeyword">in</span> oMyCurves
      <span class="HlVBSKeyword">If</span> oMyCurve.ShapeType = <span class="Hldiademconstant">e3DShapeSurface</span> <span class="HlVBSKeyword">Then</span>
        <span class="HlVBSKeyword">Set</span> oMySurfaceLine = oMyCurve.Shape.Extensions.SurfaceIsoline
        oMySurfaceLine.DisplayType = <span class="Hldiademconstant">e3DIsolineCorrespondingToIsoValueAndProjected</span>
        oMySurfaceLine.Visible = <span class="HlVBSKeyword">True</span>
        <span class="HlVBSKeyword">Call</span> oMySurfaceLine.Line.Color.SetPredefinedColor(<span class="Hldiademconstant">eColorIndexPalette</span>)
        <span class="HlVBSKeyword">Set</span> oMyColoredLines = oMyCurve.Shape.Settings.Palette
        <span class="HlVBSKeyword">For</span> i = <span class="HlNumbers">1</span> <span class="HlVBSKeyword">to</span> oMyColoredLines.Count
          oMyColoredLines(i).LineType = <span class="Hldiademconstant">eLineTypeDashDot</span> 
          oMyColoredLines(i).Width = <span class="Hldiademconstant">eLineWidth0050</span>
        <span class="HlVBSKeyword">Next</span>
      <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
    <span class="HlVBSKeyword">Next</span>
  <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
<span class="HlVBSKeyword">Next</span></donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>oMyReportObjects = dd.Report.ActiveSheet.Objects 
<span class="HlVBSKeyword">for</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects: 
    <span class="HlVBSKeyword">if</span> oMyReportObj.ObjectType == dd.eReportObject3DAxisSystem : 
        oMyCurves = oMyReportObj.Curves3D 
        <span class="HlVBSKeyword">for</span> oMyCurve <span class="HlVBSKeyword">in</span> oMyCurves: 
            <span class="HlVBSKeyword">if</span> oMyCurve.ShapeType == dd.e3DShapeSurface : 
                oMySurfaceLine = oMyCurve.Shape.Extensions.SurfaceIsoline 
                oMySurfaceLine.DisplayType = dd.e3DIsolineCorrespondingToIsoValueAndProjected 
                oMySurfaceLine.Visible = <span class="HlVBSKeyword">True</span> 
                oMySurfaceLine.Line.Color.SetPredefinedColor(dd.eColorIndexPalette) 
                oMyColoredLines = oMyCurve.Shape.Settings.Palette 
                <span class="HlVBSKeyword">for</span> i <span class="HlVBSKeyword">in</span> <span class="HlVBSKeyword">range</span>( <span class="HlNumbers">1</span>, oMyColoredLines.Count+<span class="HlNumbers">1</span>): 
                    oMyColoredLines(i).LineType = dd.eLineTypeDashDot 
                    oMyColoredLines(i).Width = dd.eLineWidth0050 
	 
</donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepD3SurfaceIsolineAdditionalInt.htm`*

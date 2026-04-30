---
title: "IRepSettingsImageExportTIFInt.BitsPerPixel"
description: "Specifies in DIAdem REPORT the color depth of a graphic exported in a TIF format."
---

# IRepSettingsImageExportTIFInt.BitsPerPixel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BitsPerPixel for SettingsImageExportTIF

Specifies in DIAdem REPORT the color depth of a graphic exported in a TIF format.

## Signature

```python
obj.BitsPerPixel
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTIFBitsPerPixelRGB1` | 0 | Black/White |
| `eTIFBitsPerPixelRGB4` | 1 | 16 colors |
| `eTIFBitsPerPixelRGB8` | 2 | 256 colors |
| `eTIFBitsPerPixelRGB16` | 3 | 65536 colors |
| `eTIFBitsPerPixelRGB24` | 4 | 24 bit RGB |
| `eTIFBitsPerPixelRGB32` | 5 | 32 bit RGB |
| `eTIFBitsPerPixelCMYK24` | 6 | 24 bit CMYK |
| `eTIFBitsPerPixelCMYK32` | 7 | 32 bit CMYK |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
OMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
OMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyTIFExport = dd.Report.Settings.ImageExport.TIF
oMyTIFExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1
oMyTIFExport.Height = 300
oMyTIFExport.UseCompression = False
oMyTIFExport.UseRatio = True
oMyTIFExport.Width = 400
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + "MyImage", dd.eImageExportTypeTIF)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMy2DAxisSystem, oMy2DCurve, oMyTIFExport
<span class="HlVBSKeyword">Call</span> <span class="Hldiademobject">Report.NewLayout</span>()
<span class="HlVBSKeyword">Set</span> oMy2DAxisSystem = <span class="Hldiademobject">Report.ActiveSheet.Objects.Add</span>(<span class="Hldiademconstant">eReportObject2DAxisSystem</span>, <span class="HlString">"My2DAxisSystem"</span>)
<span class="HlVBSKeyword">Set</span> oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(<span class="Hldiademconstant">e2DShapeLine</span>, <span class="HlString">"MyCurve"</span>)
OMy2DCurve.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span>
OMy2DCurve.Shape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span>
<span class="HlVBSKeyword">Set</span> oMyTIFExport = <span class="Hldiademobject">Report.Settings.ImageExport.TIF</span>
oMyTIFExport.BitsPerPixel = <span class="Hldiademconstant">eGIFBitsPerPixelRGB1</span>
oMyTIFExport.Height = <span class="HlNumbers">300</span>
oMyTIFExport.UseCompression = <span class="HlVBSKeyword">FALSE</span>
oMyTIFExport.UseRatio = <span class="HlVBSKeyword">TRUE</span>
oMyTIFExport.Width = <span class="HlNumbers">400</span>
<span class="HlVBSKeyword">Call</span> oMy2DAxisSystem.ExportToImage(<span class="Hldiademvariable">LayoutWritePath</span> &amp; <span class="HlString">"MyImage"</span>, <span class="Hldiademconstant">eImageExportTypeTIF</span>)</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.Report.NewLayout() 
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, <span class="HlString">"My2DAxisSystem"</span>) 
oMy2DCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, <span class="HlString">"MyCurve"</span>) 
OMy2DCurve.Shape.XChannel.Reference = <span class="HlString">"[1]/[1]"</span> 
OMy2DCurve.Shape.YChannel.Reference = <span class="HlString">"[1]/[2]"</span> 
oMyTIFExport = dd.Report.Settings.ImageExport.TIF 
oMyTIFExport.BitsPerPixel = dd.eGIFBitsPerPixelRGB1 
oMyTIFExport.Height = <span class="HlNumbers">300</span> 
oMyTIFExport.UseCompression = <span class="HlVBSKeyword">False</span> 
oMyTIFExport.UseRatio = <span class="HlVBSKeyword">True</span> 
oMyTIFExport.Width = <span class="HlNumbers">400</span> 
oMy2DAxisSystem.ExportToImage(dd.LayoutWritePath + <span class="HlString">"MyImage"</span>, dd.eImageExportTypeTIF) 
	 </donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BitsPerPixel_IRepSettingsImageExportTIFInt.htm`*

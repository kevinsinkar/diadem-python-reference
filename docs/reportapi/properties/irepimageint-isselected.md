---
title: "IRepImageInt.IsSelected"
description: "Specifies whether a graphic is selected in DIAdem REPORT."
---

# IRepImageInt.IsSelected

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IsSelected for Image

Specifies whether a graphic is selected in DIAdem REPORT.

## Signature

```python
obj.IsSelected
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
sOutput = ""
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectImage :
        sOutput = sOutput + "Object " + oMyReportObj.Name + " is selected: "+ oMyReportObj.IsSelected + "\r\n"
dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMyReportObj, oMyReportObjects, sOutput
<span class="HlVBSKeyword">Set</span> oMyReportObjects = <span class="Hldiademobject">Report.ActiveSheet.Objects</span>
sOutput = <span class="HlString">""</span>
<span class="HlVBSKeyword">For</span> <span class="HlVBSKeyword">Each</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects
  <span class="HlVBSKeyword">If</span> oMyReportObj.ObjectType = <span class="Hldiademconstant">eReportObjectImage</span> <span class="HlVBSKeyword">Then</span>
    sOutput = sOutput &amp; <span class="HlString">"Object "</span> &amp; oMyReportObj.Name &amp; <span class="HlString">" is selected: "</span>&amp; oMyReportObj.IsSelected &amp; <span class="HlVBSKeyword">VBCrLf</span>
  <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
<span class="HlVBSKeyword">Next</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">MsgBoxDisp</span>(sOutput)</donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>oMyReportObjects = dd.Report.ActiveSheet.Objects 
sOutput = <span class="HlString">""</span> 
<span class="HlVBSKeyword">for</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects: 
    <span class="HlVBSKeyword">if</span> oMyReportObj.ObjectType == dd.eReportObjectImage : 
        sOutput = sOutput + <span class="HlString">"Object "</span> + oMyReportObj.Name + <span class="HlString">" is selected: "</span>+ oMyReportObj.IsSelected + <span class="HlString">"\r\n"</span> 
dd.MsgBoxDisp(sOutput) 
	 
</donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IsSelected_IRepImageInt.htm`*

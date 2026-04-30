---
title: "IRepPolarInt.SelectedElements"
description: "Returns a collection of all selected elements of a polar axis system in DIAdem REPORT."
---

# IRepPolarInt.SelectedElements

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SelectedElements for PolarSystem

Returns a collection of all selected elements of a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.SelectedElements
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObjectPolarSystem :
        oMySelection = oMyReportObj.SelectedElements
        sOutput = "Object name: " + oMyReportObj.Name + "\r\n" +"Number of selected elements: " + oMySelection.Count + "\r\n"
        for i in range( 1, oMySelection.Count+1):
            sOutput = sOutput + "Element type: " + oMySelection.Item(i).Type + "\r\n"
        dd.MsgBoxDisp(sOutput)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p>
</div>
<div class="codeblue" contenteditable="false">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMyReportObj, oMyReportObjects, oMySelection, sOutput, i
<span class="HlVBSKeyword">Set</span> oMyReportObjects = <span class="Hldiademobject">Report.ActiveSheet.Objects</span>
<span class="HlVBSKeyword">For</span> <span class="HlVBSKeyword">Each</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects
  <span class="HlVBSKeyword">If</span> oMyReportObj.ObjectType = <span class="Hldiademconstant">eReportObjectPolarSystem</span> <span class="HlVBSKeyword">Then</span>
    <span class="HlVBSKeyword">Set</span> oMySelection = oMyReportObj.SelectedElements
    sOutput = <span class="HlString">"Object name: "</span> &amp; oMyReportObj.Name &amp; <span class="HlVBSKeyword">vbCrLf</span> &amp;_
              <span class="HlString">"Number of selected elements: "</span> &amp; oMySelection.Count &amp; <span class="HlVBSKeyword">vbCrLf</span>
    <span class="HlVBSKeyword">For</span> i = <span class="HlNumbers">1</span> <span class="HlVBSKeyword">to</span> oMySelection.Count
      sOutput = sOutput &amp; <span class="HlString">"Element type: "</span> &amp; oMySelection.Item(i).Type &amp; <span class="HlVBSKeyword">vbCrLf</span>
    <span class="HlVBSKeyword">Next</span>
    <span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">MsgBoxDisp</span>(sOutput)
  <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
<span class="HlVBSKeyword">Next</span></donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>oMyReportObjects = dd.Report.ActiveSheet.Objects 
<span class="HlVBSKeyword">for</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects: 
    <span class="HlVBSKeyword">if</span> oMyReportObj.ObjectType == dd.eReportObjectPolarSystem : 
        oMySelection = oMyReportObj.SelectedElements 
        sOutput = <span class="HlString">"Object name: "</span> + oMyReportObj.Name + <span class="HlString">"\r\n"</span> +<span class="HlString">"Number of selected elements: "</span> + oMySelection.Count + <span class="HlString">"\r\n"</span> 
        <span class="HlVBSKeyword">for</span> i <span class="HlVBSKeyword">in</span> <span class="HlVBSKeyword">range</span>( <span class="HlNumbers">1</span>, oMySelection.Count+<span class="HlNumbers">1</span>): 
            sOutput = sOutput + <span class="HlString">"Element type: "</span> + oMySelection.Item(i).Type + <span class="HlString">"\r\n"</span> 
        dd.MsgBoxDisp(sOutput) 
	 
</donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SelectedElements_IRepPolarInt.htm`*

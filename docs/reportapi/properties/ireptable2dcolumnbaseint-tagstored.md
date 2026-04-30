---
title: "IRepTable2DColumnBaseInt.TagStored"
description: "Specifies a tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a"
---

# IRepTable2DColumnBaseInt.TagStored

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TagStored for 2DTableColumn

Specifies a tag for an object in DIAdem REPORT. Use this property to add additional information to the object. Afterwards you can evaluate such information in a program, for example, for special treatment of the object. The tag does not affect the behavior of the object. DIAdem saves this tag with the layout.

## Signature

```python
obj.TagStored
```

## Python example

```python
oMyReportObjects = dd.Report.ActiveSheet.Objects
for oMyReportObj in oMyReportObjects:
    if oMyReportObj.ObjectType == dd.eReportObject2DTable :
        oMySubObjects = oMyReportObj.Columns
        for oMySubObj in oMySubObjects:
            oMySubObj.TagStored = "Column type: " + oMySubObj.Type
```

## See also

<div markdown="1">
<div class="SeeAlso">
<p class="body">The following example assigns a tag to a table column:</p><table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div><div class="codeblue"><pre><donottranslate><span class="HlVBSKeyword">Dim</span> oMyReportObj, oMyReportObjects, oMySubObjects, oMySubObj
<span class="HlVBSKeyword">Set</span> oMyReportObjects = <span class="Hldiademobject">Report.ActiveSheet.Objects</span>
<span class="HlVBSKeyword">For</span> <span class="HlVBSKeyword">Each</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects
  <span class="HlVBSKeyword">If</span> oMyReportObj.ObjectType = <span class="Hldiademconstant">eReportObject2DTable</span> <span class="HlVBSKeyword">Then</span>
    <span class="HlVBSKeyword">Set</span> oMySubObjects = oMyReportObj.Columns
    <span class="HlVBSKeyword">For</span> <span class="HlVBSKeyword">Each</span> oMySubObj <span class="HlVBSKeyword">in</span> oMySubObjects
      oMySubObj.TagStored = <span class="HlString">"Column type: "</span> &amp; oMySubObj.Type
    <span class="HlVBSKeyword">Next</span>
  <span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">If</span>
<span class="HlVBSKeyword">Next</span></donottranslate></pre></div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>oMyReportObjects = dd.Report.ActiveSheet.Objects 
<span class="HlVBSKeyword">for</span> oMyReportObj <span class="HlVBSKeyword">in</span> oMyReportObjects: 
    <span class="HlVBSKeyword">if</span> oMyReportObj.ObjectType == dd.eReportObject2DTable : 
        oMySubObjects = oMyReportObj.Columns 
        <span class="HlVBSKeyword">for</span> oMySubObj <span class="HlVBSKeyword">in</span> oMySubObjects: 
            oMySubObj.TagStored = <span class="HlString">"Column type: "</span> + oMySubObj.Type 
</donottranslate></pre></div>
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TagStored_IRepTable2DColumnBaseInt.htm`*

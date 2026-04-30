---
title: "IRepReportInt"
description: "The Report object provides access to the objects in DIAdem REPORT. You can also use the Report object to specify the general properties of DIAdem REPORT. The Re"
---

# IRepReportInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Report

The Report object provides access to the objects in DIAdem REPORT. You can also use the Report object to specify the general properties of DIAdem REPORT. The Report object is available as a global object in scripts and in dialog boxes. Do not create an object or a variable with the name Report because this overwrites the Report object.

## Python example

```python
dd.Report.NewLayout()
oMyComment = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectComment,"MyComment")
oMyComment.Comment.Text = "This is a comment"
oMyFont = oMyComment.Comment.Font
oMyFont.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFont.Name = "Tahoma"
oMyFont.Size = 7
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepreportint-activesheet/">ActiveSheet</a> | <a href="../../properties/irepreportint-appendedfilename/">AppendedFileName</a> | <a href="../../properties/irepreportint-appendedfullpath/">AppendedFullPath</a> | <a href="../../properties/irepreportint-comment/">Comment</a> | <a href="../../properties/irepreportint-events/">Events</a> | <a href="../../properties/irepreportint-filename/">FileName</a> | <a href="../../properties/irepreportint-fullpath/">FullPath</a> | <a href="../../properties/irepreportint-selectedobjects/">SelectedObjects</a> | <a href="../../properties/irepreportint-settings/">Settings</a> | <a href="../../properties/irepreportint-sheets/">Sheets</a> | <a href="../../properties/irepreportint-tagstored/">TagStored</a> | <a href="../../properties/irepreportint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepreportint-appendlayout/">AppendLayout</a> | <a href="../../methods/irepreportint-ismasterlayout/">IsMasterLayout</a> | <a href="../../methods/irepreportint-ismodified/">IsModified</a> | <a href="../../methods/irepreportint-loadlayout/">LoadLayout</a> | <a href="../../methods/irepreportint-loadmasterlayout/">LoadMasterLayout</a> | <a href="../../methods/irepreportint-newlayout/">NewLayout</a> | <a href="../../methods/irepreportint-newmasterlayout/">NewMasterLayout</a> | <a href="../../methods/irepreportint-refresh/">Refresh</a> | <a href="../../methods/irepreportint-refreshsilent/">RefreshSilent</a> | <a href="../../methods/irepreportint-resetmodified/">ResetModified</a> | <a href="../../methods/irepreportint-savelayout/">SaveLayout</a> | <a href="../../methods/irepreportint-savemasterlayout/">SaveMasterLayout</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepReportInt.htm`*

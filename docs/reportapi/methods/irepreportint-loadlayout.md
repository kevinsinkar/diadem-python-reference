---
title: "IRepReportInt.LoadLayout"
description: "Loads the specified layout in DIAdem REPORT. Layouts have the filename extension *.tdr or *.tdrz ."
---

# IRepReportInt.LoadLayout

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: LoadLayout for Report

Loads the specified layout in DIAdem REPORT. Layouts have the filename extension *.tdr or *.tdrz .

## Signature

```python
obj.LoadLayout(FileName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If you do not specify a path with the filename, DIAdem uses the REPORT user path.</td></tr></table>
</div>

## Python example

```python
dd.Report.LoadLayout("Example.tdr")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_LoadLayout_IRepReportInt.htm`*

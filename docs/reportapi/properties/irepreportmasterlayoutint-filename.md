---
title: "IRepReportMasterLayoutInt.FileName"
description: "Specifies the name of the current master layout in DIAdem REPORT. The name can include DIAdem expressions ."
---

# IRepReportMasterLayoutInt.FileName

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: FileName for MasterLayout

Specifies the name of the current master layout in DIAdem REPORT. The name can include DIAdem expressions .

## Signature

```python
obj.FileName
```

## Python example

```python
dd.Report.NewLayout()
oMyMasterLayout = dd.Report.Settings.MasterLayout
oMyMasterLayout.Connect("Example.tdrm")
dd.MsgBoxDisp("Name: " + oMyMasterLayout.FileName + "\r\n" + "Path: " + oMyMasterLayout.FullPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_FileName_IRepReportMasterLayoutInt.htm`*

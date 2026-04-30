---
title: "IRepReportInt.AppendedFileName"
description: "Specifies the file name of a layout loaded to the existing layout in DIAdem REPORT."
---

# IRepReportInt.AppendedFileName

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AppendedFileName for Report

Specifies the file name of a layout loaded to the existing layout in DIAdem REPORT.

## Signature

```python
obj.AppendedFileName
```

## Python example

```python
dd.Report.AppendLayout("Demo.tdr")
print("Fullpath: " + dd.Report.AppendedFullPath + "\r\n" + "Layout file name: " + dd.Report.AppendedFileName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AppendedFileName_IRepReportInt.htm`*

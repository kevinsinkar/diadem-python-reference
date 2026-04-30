---
title: "IRepSheetListInt.ShowPrintDlg"
description: "Displays the printer dialog box in DIAdem REPORT. The method sets the variable DlgState . DlgState contains the status of the dialog box after you exit the dial"
---

# IRepSheetListInt.ShowPrintDlg

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ShowPrintDlg for Sheets

Displays the printer dialog box in DIAdem REPORT. The method sets the variable DlgState . DlgState contains the status of the dialog box after you exit the dialog box.

## Signature

```python
obj.ShowPrintDlg()
```

## Python example

```python
dd.Report.Sheets.ShowPrintDlg()
if dd.DlgState != "IDOk" :
    print("Sheet was not printed.")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_ShowPrintDlg_IRepSheetListInt.htm`*

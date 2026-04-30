---
title: "IRepTextSimpleInt.BackgroundColor"
description: "Specifies the background color of a text in DIAdem REPORT."
---

# IRepTextSimpleInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for Text

Specifies the background color of a text in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
```

## Python example

```python
dd.Report.NewLayout()
oMyText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectText,"MyText")
oMyText.Text = "MyText"
dd.MsgBoxDisp(oMyText.BackgroundColor.RGB)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepTextSimpleInt.htm`*

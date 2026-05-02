---
title: "IRepReportEventsInt"
description: "The Events object provides events in DIAdem REPORT."
---

# IRepReportEventsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: Events

The Events object provides events in DIAdem REPORT.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Refer to <a href="#" data-unresolved="1">Working with Events in DIAdem</a> for further information.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.AddUserCommandToEvent("dd.Report.Events.OnFinalizeSheetRefresh","MyOnFinalizeSheetRefresh")

def MyOnFinalizeSheetRefresh(Sheet):
    dd.MsgBox("Sheet: " + Sheet.Name + "\t" + "Number of objects: " + Sheet.Objects.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepreporteventsint-clickedwithkey/">ClickedWithKey</a> | <a href="../../properties/irepreporteventsint-drawing/">Drawing</a> | <a href="../../properties/irepreporteventsint-drop/">Drop</a> | <a href="../../properties/irepreporteventsint-oncontextmenupointselected/">OnContextMenuPointSelected</a> | <a href="../../properties/irepreporteventsint-onfinalizesheetrefresh/">OnFinalizeSheetRefresh</a> | <a href="../../properties/irepreporteventsint-oninitializesheetrefresh/">OnInitializeSheetRefresh</a> | <a href="../../properties/irepreporteventsint-onlayoutloaded/">OnLayoutLoaded</a> | <a href="../../properties/irepreporteventsint-onlayoutsaving/">OnLayoutSaving</a> | <a href="../../properties/irepreporteventsint-onshowingcontextmenu/">OnShowingContextMenu</a> | <a href="../../properties/irepreporteventsint-tooltip/">ToolTip</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepreportint/">Report</a>.<a href="../../properties/irepreportint-events/">Events</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepReportEventsInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

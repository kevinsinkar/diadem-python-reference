---
title: "IRepTable2DDropContextInt"
description: "The 2DTableDropContext object provides information about the 2D axis system onto which you dragged and dropped an object. Do not set the DoProceed property to T"
---

# IRepTable2DDropContextInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DTableDropContext

The 2DTableDropContext object provides information about the 2D axis system onto which you dragged and dropped an object. Do not set the DoProceed property to TRUE if you change the number of columns in the associated event or if you execute similar operations.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
AddUserCommandToEvent("dd.Report.Events.OnDrop2DTable", "MyOnDrop2DTableEvent")

def MyOnDrop2DTableEvent(Context, DropContext):
    sOutput = "Names of dropped channels:"
    for oMyDropElement in DropContext.DiademElements:
        sOutput = sOutput + "\r\n" + oMyDropElement.Name
    Msgbox(sOutput)
    oMyTable = Context.Table
    if Context.ColumnIndex>0:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyTable.Name + "\r\n" + oMyTable.Columns.Item(Context.ColumnIndex).Type)
    else:
        dd.MsgBox(Context.Sheet.Name + "\r\n" + oMyTable.Name)
    Context.DoProceed = TRUE
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptable2ddropcontextint-columnindex/">ColumnIndex</a> | <a href="../../properties/ireptable2ddropcontextint-doproceed/">DoProceed</a> | <a href="../../properties/ireptable2ddropcontextint-sheet/">Sheet</a> | <a href="../../properties/ireptable2ddropcontextint-table/">Table</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTable2DDropContextInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

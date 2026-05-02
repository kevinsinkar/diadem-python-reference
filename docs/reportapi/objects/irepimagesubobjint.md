---
title: "IRepImageSubObjInt"
description: "The ImageSubObj object provides information about a subobject of a graphic in DIAdem REPORT when DIAdem calls the event assigned to the OnImage for ToolTipEvent"
---

# IRepImageSubObjInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ImageSubObj

The ImageSubObj object provides information about a subobject of a graphic in DIAdem REPORT when DIAdem calls the event assigned to the OnImage for ToolTipEvents property. DIAdem calls this event if you press the shift key and move the mouse over a REPORT object.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>To test the example script, you must first save the second script and register it as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
dd.Report.NewLayout()
oMyImage = dd.Report.ActiveSheet.Objects.Add(eReportObjectImage, "MyImage")
oMyPos = oMyImage.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyImage.FileName = MediaLibrPath + "Example1.png"
oMyImage.BackgroundColor.SetPredefinedColor(eColorIndexNone)

# This event will be raised if the mouse is moved AND the shift key pressed
dd.Report.Events.ToolTip.OnImage = "MyToolTipEvent"
dd.Report.Refresh()
```

```python
def MyToolTipEvent(Context,ToolTipText):
    oSubObject = Context.SubObject
    ToolTipText = "Sheet: " + Context.Sheet.Name + "\r\n" + "Sub object" + "\r\n" + "Name: " + oSubObject.Name + "\r\n" + "Type: " + GetConstNameForREPORTSubObj(oSubObject, oSubObject.Type)
    ToolTipText = ToolTipText + "\r\n" + "X position: " + Context.Position.X + "\r\n" + "Y position: " + Context.Position.Y
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepimagesubobjint-name/">Name</a> | <a href="../../properties/irepimagesubobjint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireptooltipimagecontextint/">ToolTipImageContext</a>.<a href="../../properties/ireptooltipimagecontextint-subobject/">SubObject</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepImageSubObjInt.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

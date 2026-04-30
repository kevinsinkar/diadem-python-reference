---
title: "IRepTextObjectInt"
description: "The RTFText object provides access to a Text Object in DIAdem-REPORT."
---

# IRepTextObjectInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: RTFText

The RTFText object provides access to a Text Object in DIAdem-REPORT.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>With the object-oriented script interface in DIAdem REPORT, you can only create, position, and select text objects. You cannot create and change text in text objects.</td></tr></table>
</div>

## Python example

```python
dd.Report.NewLayout()
oMyRTFText = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectRTFText,"MyRtfText")
oMyRTFTextPosition = oMyRTFText.Position
oMyRTFTextPosition.ByCoordinate.X1 = 100
oMyRTFTextPosition.ByCoordinate.X2 = 30
oMyRTFTextPosition.ByCoordinate.Y1 = 10
oMyRTFTextPosition.ByCoordinate.Y2 = 10
oMyRTFText.ExportToImage("MyRtfText",dd.eImageExportTypePNG)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireptextobjectint-index/">Index</a> | <a href="../../properties/ireptextobjectint-isselected/">IsSelected</a> | <a href="../../properties/ireptextobjectint-name/">Name</a> | <a href="../../properties/ireptextobjectint-objecttype/">ObjectType</a> | <a href="../../properties/ireptextobjectint-position/">Position</a> | <a href="../../properties/ireptextobjectint-tagstored/">TagStored</a> | <a href="../../properties/ireptextobjectint-tagtemporary/">TagTemporary</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/ireptextobjectint-exporttoimage/">ExportToImage</a> | <a href="../../methods/ireptextobjectint-select/">Select</a> | <a href="../../methods/ireptextobjectint-showpropertiesdlg/">ShowPropertiesDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-add/">Add</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-copy/">Copy</a> | <a href="../../collections/reportobjects/">ReportObjects</a>.<a href="../../methods/irepctrllistint-item/">Item</a> | <a href="../../collections/selectedobjects/">SelectedObjects</a>.<a href="../../methods/irepselectedobjectslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepTextObjectInt.htm`*

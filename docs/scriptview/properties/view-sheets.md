---
title: "VIEW.Sheets"
description: "Returns a Worksheets collection in DIAdem VIEW."
---

# VIEW.Sheets

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Sheets for View

Returns a Worksheets collection in DIAdem VIEW.

## Signature

```python
return_value = obj.Sheets
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Unlike manual operation, you can delete all worksheets in scripts.</td></tr></table>
</div>

## Python example

```python
for oMySheet in dd.View.Sheets:
    dd.MsgBoxDisp(oMySheet.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Sheets_VIEW.htm`*

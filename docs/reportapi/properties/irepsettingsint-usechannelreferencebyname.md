---
title: "IRepSettingsInt.UseChannelReferenceByName"
description: "Specifies that DIAdem REPORT uses channel names for channel assignments."
---

# IRepSettingsInt.UseChannelReferenceByName

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseChannelReferenceByName for Settings

Specifies that DIAdem REPORT uses channel names for channel assignments.

## Signature

```python
obj.UseChannelReferenceByName
```

## Python example

```python
dd.MsgBoxDisp(dd.Report.Settings.UseChannelReferenceByName)
```

```python
dd.Data.Root.Clear()
if (dd.FileNameGet("NAVIGATOR", "FileRead", dd.DataReadPath + ".TDM") == "IDOk") : # Dialog closed with Ok
    if dd.FileDlgPartial :
# Open dialog to select channels, then load or register
        dd.DataFileSelDlg(dd.FileDlgFileName,dd.FileDlgFilter)
    else:
# Load or register all channels
        dd.DataFileLoad(dd.FileDlgFileName,dd.FileDlgFilter,dd.FileDlgImpAction)
dd.Report.Settings.ConvertToChannelReferenceByName()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseChannelReferenceByName_IRepSettingsInt.htm`*

---
title: "IRepSettingsInt.ConvertToChannelReferenceByName"
description: "Converts a layout in DIAdem-REPORT into a name-oriented layout. The channel name is used as channel reference in the layout. Before executing the command you mu"
---

# IRepSettingsInt.ConvertToChannelReferenceByName

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: ConvertToChannelReferenceByName for Settings

Converts a layout in DIAdem-REPORT into a name-oriented layout. The channel name is used as channel reference in the layout. Before executing the command you must load a suitable data set so that the channel reference is correct. As of version 2019, DIAdem does not support channel numbers. For this reason you can access the property UseChannelReferenceByName only in read-only mode. To convert a number-oriented layout correctly into a name-oriented layout, load the layout to be converted in DIAdem 2018 or earlier, load a suitable data set, and execute the method ConvertToChannelReferenceByName .

## Signature

```python
obj.ConvertToChannelReferenceByName()
```

## Python example

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

*Source: `ReportApi/methods/Report_method_ConvertToChannelReferenceByName_IRepSettingsInt.htm`*

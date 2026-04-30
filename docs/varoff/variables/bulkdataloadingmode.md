---
title: "BulkDataLoadingMode"
description: "Specifies when DIAdem loads bulk data into the Data Portal."
---

# BulkDataLoadingMode

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: BulkDataLoadingMode:

Specifies when DIAdem loads bulk data into the Data Portal.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the Help page on <a href="#" data-unresolved="1">Loading Bulk Data - General</a> for more information about loading bulk data in DIAdem.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBulkDataLoadingImmediately` | 24120 | Always load bulk data |
| `eBulkDataLoadingOnFirstAccess` | 24121 | Load bulk data on first access |
| `eBulkDataLoadingOnWriteAccess` | 24122 | Load bulk data on modification of channel data |

## Python example

```python
def BulkDataLoadingModeToText(mode):
    select_variable_0 = mode
    if (select_variable_0 == dd.eBulkDataLoadingImmediately) :
        BulkDataLoadingModeToText = "Always load bulk data"
    elif (select_variable_0 == dd.eBulkDataLoadingOnFirstAccess) :
        BulkDataLoadingModeToText = "Load bulk data on first access"
    elif (select_variable_0 == dd.eBulkDataLoadingOnWriteAccess) :
        BulkDataLoadingModeToText = "Load bulk data on modification of channel data"
    else:
        BulkDataLoadingModeToText = "-- illegal mode --"
    return BulkDataLoadingModeToText
```

---

*Source: `VarOff/BulkDataLoadingMode.htm`*

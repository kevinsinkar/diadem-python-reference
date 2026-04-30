---
title: "SFD_GetScan"
description: "Requests the measurement data of a complete scan from the connected device in the script driver and saves the data in the respective variables of the script. DI"
---

# SFD_GetScan

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_GetScan

Requests the measurement data of a complete scan from the connected device in the script driver and saves the data in the respective variables of the script. DIAdem calls the SFD_GetScan function once per measurement cycle. This function simplifies receiving data from a measurement device that always provides the data for a complete scan.

## Signature

```python
dd.SFD_GetScan(ErrorP)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  This function is optional.</td></tr></table>
</div>

---

*Source: `Gfsvbsdr/sfd_getscan.htm`*

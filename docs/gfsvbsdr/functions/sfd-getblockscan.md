---
title: "SFD_GetBlockScan"
description: "Requests in the Script driver several scans in the measurement mode Hardware clock from the connected device and saves the data in the specified variable field."
---

# SFD_GetBlockScan

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_GetBlockScan

Requests in the Script driver several scans in the measurement mode Hardware clock from the connected device and saves the data in the specified variable field.

## Signature

```python
dd.SFD_GetBlockScan(ChannelNumbersV, ChannelParamsV, MaxScansV, DataP, dataIsSortedByScanP, ErrorP)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  This function must be used when data is acquired with the script driver in the measurement mode.</td></tr></table>
</div>

---

*Source: `Gfsvbsdr/sfd_getblockscan.htm`*

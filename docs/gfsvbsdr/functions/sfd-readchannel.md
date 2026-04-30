---
title: "SFD_ReadChannel"
description: "Transfers the measurement data of a single channel from the script to the script driver . The function can request the data of this channel directly from the me"
---

# SFD_ReadChannel

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_ReadChannel

Transfers the measurement data of a single channel from the script to the script driver . The function can request the data of this channel directly from the measurement device or from the respective script variables. Before the function can request measurement data from variables, the SFD_GetScan function must save the measurement data in variables, read out the data, and transfer the measurement data to the script driver. DIAdem calls this function once per measurement cycle for every active measurement channel.

## Signature

```python
dd.SFD_ReadChannel(ChannelNumberP, ParamP, DataP, ErrorP)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  This function must be used when data is acquired with the script driver in the single value mode.</td></tr></table>
</div>

---

*Source: `Gfsvbsdr/sfd_readchannel.htm`*

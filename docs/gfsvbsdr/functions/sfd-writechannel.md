---
title: "SFD_WriteChannel"
description: "Transfers measured values from the script driver for output to the script. The function can transfer the measurement values either directly to the connected dev"
---

# SFD_WriteChannel

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_WriteChannel

Transfers measured values from the script driver for output to the script. The function can transfer the measurement values either directly to the connected device or save the values in the respective variables of the script. If the function saves the measurement values in variables, the SFD_SendScan function can transfer the measurement values as a complete scan to the device. DIAdem calls this function once in each measurement cycle for each active output channel.

## Signature

```python
dd.SFD_WriteChannel(ChannelNumberP, ParamP, DataP, ErrorP)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You must use this function for data output.</td></tr></table>
</div>

---

*Source: `Gfsvbsdr/sfd_writechannel.htm`*

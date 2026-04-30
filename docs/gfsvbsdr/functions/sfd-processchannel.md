---
title: "SFD_ProcessChannel"
description: "Offsets the data of the connected input signals against each other in the script driver . DIAdem calls this function once per measurement cycle for each channel"
---

# SFD_ProcessChannel

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_ProcessChannel

Offsets the data of the connected input signals against each other in the script driver . DIAdem calls this function once per measurement cycle for each channel in the block.

## Signature

```python
dd.SFD_ProcessChannel(ChannelNumberP, InputListV, ParamP, DataP, ErrorP)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You must use this function for scripts that output data.</td></tr></table>
</div>

---

*Source: `Gfsvbsdr/sfd_processchannel.htm`*

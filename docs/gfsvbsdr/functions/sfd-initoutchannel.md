---
title: "SFD_InitOutChannel"
description: "Initializes the required output channels in the script driver . DIAdem calls the SFD_InitOutChannel function during the measurement preparation, once for every "
---

# SFD_InitOutChannel

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_InitOutChannel

Initializes the required output channels in the script driver . DIAdem calls the SFD_InitOutChannel function during the measurement preparation, once for every active output.

## Signature

```python
dd.SFD_InitOutChannel(ChannelNumberP, ParamP, ErrorP, [ScalingFactorP], [ScalingOffsetP], [ChannelCountV])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  This function is optional.</td></tr></table>
</div>

---

*Source: `Gfsvbsdr/sfd_initoutchannel.htm`*

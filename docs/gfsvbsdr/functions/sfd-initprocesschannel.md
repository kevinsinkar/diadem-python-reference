---
title: "SFD_InitProcessChannel"
description: "Initializes the required channels for data processing in the script driver . DIAdem calls the SFD_InitProcessChannel function during the measurement preparation"
---

# SFD_InitProcessChannel

!!! abstract "Function &middot; `Gfsvbsdr.chm`"
    Function: SFD_InitProcessChannel

Initializes the required channels for data processing in the script driver . DIAdem calls the SFD_InitProcessChannel function during the measurement preparation, once for every active data processing channel.

## Signature

```python
dd.SFD_InitProcessChannel( ChannelNumberP, InputListV, ParamP, ErrorP, [ScalingFactorP], [ScalingOffsetP], [ChannelCountV], [UnitP], [PropertyListP])
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  This function is optional.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def SFD_InitProcessChannel(ChannelNumberP, InputListV, ParamP, ErrorP , ScalingFactorP, ScalingOffsetP , ChannelCountV, UnitP, PropertyListP):
    aProperties(0) = "PropertyTypeInteger"
    aProperties(1) = "MyInteger"
    aProperties(2) = 5
    aProperties(3) = "PropertyTypeString"
    aProperties(4) = "MyString"
    aProperties(5) = "This is the string value"
    PropertyListP = aProperties
```

---

*Source: `Gfsvbsdr/sfd_initprocesschannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

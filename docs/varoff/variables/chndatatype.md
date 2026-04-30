---
title: "ChnDataType"
description: "Specifies the preferred channel type with which DIAdem saves channels."
---

# ChnDataType

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ChnDataType

Specifies the preferred channel type with which DIAdem saves channels.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Notice  </strong> Not all file formats support implicit channels. For these formats, they are stored as explicit channels even if ChnDataType specifies the channel type <span class="Monospace">IMPLICIT</span>. For a description of the channel types, see the following help page: <a href="#" data-unresolved="1">channel types</a></td></tr>
</table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Notice  </strong> After an implicit channel has been expanded into an explicit channel, it is saved again as an implicit channel, if possible, in order to use as little disk space as possible. If you want to save this channel as an explicit channel, set the ChnDataType variable to <span class="Monospace">EXPLICIT</span> before saving.</td></tr>
</table>
</div>

---

*Source: `VarOff/ChnDataType.htm`*

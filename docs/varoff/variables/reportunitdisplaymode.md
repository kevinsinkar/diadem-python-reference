---
title: "ReportUnitDisplayMode"
description: "Specifies the display mode for the unit for axis labels in DIAdem REPORT if the unit is defined as a DIAdem expression in the label text with square brackets. A"
---

# ReportUnitDisplayMode

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ReportUnitDisplayMode

Specifies the display mode for the unit for axis labels in DIAdem REPORT if the unit is defined as a DIAdem expression in the label text with square brackets. A DIAdem expression , such as [@@ChnDim(CurrChnNo)@@] , is replaced by the representation of the set mode.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  The mode has no function if there is no expression for the unit in the axis label text or if it is not enclosed in square brackets.</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  The following expressions for the unit are replaced by the mode: ChnDim, CD, UnitSymbol.</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  In <span class="Monospace">ReportUnitDisplayMode5</span> mode, the combination of the channel name and the unit with the word <span class="Italic">in</span> is used as a scheme, so that no translation takes place.</td></tr>
</table>
</div>

---

*Source: `VarOff/ReportUnitDisplayMode.htm`*

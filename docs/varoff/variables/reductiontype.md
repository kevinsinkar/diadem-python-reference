---
title: "ReductionType"
description: "Specifies the data reduction method. You can select several reduction methods simultaneously. DIAdem creates a new data channel for each reduction method."
---

# ReductionType

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: ReductionType

Specifies the data reduction method. You can select several reduction methods simultaneously. DIAdem creates a new data channel for each reduction method.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">ReductionType</span> variable can accept one of the values that results from the bitwise comparison (<a href="#" data-unresolved="1">Or operator</a>) of the following constant values: <a href="../einterfirstvalue/">eInterFirstValue</a> (1), <a href="../einterminimum/">eInterMinimum</a> (2), <a href="../eintermaximum/">eInterMaximum</a> (4), <a href="../eintermeanvalue/">eInterMeanValue</a> (8)</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem creates a new data channel for each reduction method. To do this, DIAdem appends the following text to the original channel name:<table class="Borderless"><tr><td width="150"><strong>Reduction method</strong></td><td width="150"><strong>Constant</strong></td><td><strong>Channel name suffix</strong></td></tr><tr><td width="150">1. Value</td><td width="150"><a href="../einterfirstvalue/">eInterFirstValue</a> (1)</td><td>_Sample</td></tr><tr><td width="150">Minimum</td><td width="150"><a href="../einterminimum/">eInterMinimum</a> (2)</td><td>_Min</td></tr><tr><td width="150">Maximum</td><td width="150"><a href="../eintermaximum/">eInterMaximum</a> (4)</td><td>_Max</td></tr><tr><td width="150">Arithmetic mean</td><td width="150"><a href="../eintermeanvalue/">eInterMeanValue</a> (8)</td><td>_Mean</td></tr></table>
</td></tr></table>
</div>

---

*Source: `VarOff/ReductionType.htm`*

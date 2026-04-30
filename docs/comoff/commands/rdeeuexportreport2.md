---
title: "RdeEuExportReport2"
description: "Exports the end results of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November"
---

# RdeEuExportReport2

!!! abstract "Command &middot; `ComOff.chm`"
    Command: RdeEuExportReport2

Exports the end results of the RdeEuAnalysis data evaluation according to the data exchange format described in Commission Regulation (EU) 2018/1832 of November 5, 2018, Annex III, Appendix 8, Point 4.2.2, Table 4, 5, 5a, 5b, and 6. The command assumes that the metadata is stored as group properties of the first channel group.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">TargetFile</td>
<td>Specifies the name of a data file with the filename extension and the path.<div id="exp_TargetFile"><table class="Borderless">
<tr><td width="150"><a href="#" data-unresolved="1">String variable</a></td></tr>
</table></div>
</td></tr>
<tr><td width="150">TargetLanguage</td>
<td>Specifies the language of the exported file.<div id="exp_TargetLanguage"><table class="Borderless">
<tr><td width="150"><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr><td>The following settings are possible:<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"english"</pre></donottranslate></td>
<td>English</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150">
<donottranslate><span class="Monospace"><em>ReturnValue</em></span></donottranslate></td>
<td>Returns the value <span class="Monospace">0</span> if the function has executed successfully. Returns a negative value if an error occurred.</td>
</tr>
</table>
</div>

---

*Source: `ComOff/RdeEuExportReport2.htm`*

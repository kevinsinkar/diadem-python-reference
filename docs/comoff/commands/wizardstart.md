---
title: "WizardStart"
description: "Starts a wizard."
---

# WizardStart

!!! abstract "Command &middot; `ComOff.chm`"
    Command: WizardStart

Starts a wizard.

## Signature

```python
dd.WizardStart([WIZName], [WIZPageName], [WIZParam])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[WIZName]</td>
<td>Specifies the name of a wizard.<div id="exp_WIZName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">You can select from the following options:</p>
<table class="Borderless"><tr><td width="150"><span class="Monospace">WizChart</span></td><td>Specifies the <a href="#" data-unresolved="1">Chart Wizard</a></td></tr><tr><td width="150"><span class="Monospace">WizReport</span></td><td>Specifies the <a href="#" data-unresolved="1">Report Wizard</a></td></tr><tr><td width="150"><span class="Monospace">WizDataPlugin</span></td><td>Specifies the <a href="#" data-unresolved="1">DataPlugin Wizard</a></td></tr></table>
<p class="Body">The default setting for the <span class="Monospace">Wizname</span> variable is <span class="Monospace">WizReport</span>.</p>
</div></td></tr>
<tr><td width="150">[WIZPageName]</td>
<td>Specifies the start page for a wizard.<div id="exp_WIZPageName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">The DIAdem <a href="#" data-unresolved="1">Chart Wizard</a> and the DIAdem <a href="#" data-unresolved="1">DataPlugin Wizard</a> do not use this parameter.</p>
<p class="Body">In the DIAdem <a href="#" data-unresolved="1">Report Wizard</a> you can use the start pages <span class="Monospace">INTRODUCTION</span>, <span class="Monospace">CURVEUSAGE</span>, and <span class="Monospace">LAYOUTSTYLE</span>. The default setting for the <span class="Monospace">WizPageName</span> variable is <span class="Monospace">INTRODUCTION</span>.</p>
</div></td></tr>
<tr><td width="150">[WIZParam]</td>
<td>Specifies further parameters of a wizard.<div id="exp_WIZParam">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">The DIAdem <a href="#" data-unresolved="1">Chart Wizard</a> and the DIAdem <a href="#" data-unresolved="1">DataPlugin Wizard</a> do not use this parameter.</p>
<p class="Body">DIAdem uses the <span class="Monospace">WizParam</span> variable in the diagram wizard to recognize a call, for example, from the Data Portal. In this case <span class="Monospace">WizParam</span> has the value <span class="Monospace">&lt;callorigin&gt;PORTAL&lt;/callorigin&gt;</span>.</p>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.WizardStart("WizChart")
```

---

*Source: `ComOff/WizardStart.htm`*

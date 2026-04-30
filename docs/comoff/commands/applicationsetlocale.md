---
title: "ApplicationSetLocale"
description: "Switches country specific variables and quantities. The affected variables are TimeFormat and LengthUnit . The paper format and the margins belong to the countr"
---

# ApplicationSetLocale

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ApplicationSetLocale

Switches country specific variables and quantities. The affected variables are TimeFormat and LengthUnit . The paper format and the margins belong to the country specific quantities. If you use the ApplicationSetLocale command in a simulation of the analysis automation or of the data preparation, DIAdem uses the settings only while the script is running.

## Signature

```python
dd.ApplicationSetLocale( ApplicationLocale )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The <span class="Monospace">ApplicationSetLocale</span> command does not influence the country-specific settings of the interface. However, the command does influence the country-specific settings during script runtime.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ApplicationLocale</td>
<td>Specifies to which locale to switch the variables and quantities. If the language of the <span class="Monospace">operating system</span> does not correspond with any language on the list, DIAdem uses <span class="Monospace">English</span>.<div id="exp_ApplicationLocale">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"operating system"</pre></donottranslate></td>
<td>Operating system language</td></tr>
<tr><td width="150"><donottranslate><pre>"german"</pre></donottranslate></td>
<td>German</td></tr>
<tr><td width="150"><donottranslate><pre>"english"</pre></donottranslate></td>
<td>English</td></tr>
<tr><td width="150"><donottranslate><pre>"japanese"</pre></donottranslate></td>
<td>Japanese</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ApplicationSetLocale.htm`*

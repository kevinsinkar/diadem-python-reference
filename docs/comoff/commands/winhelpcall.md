---
title: "WinHelpCall"
description: "Opens a help file with the extension .hlp or .chm."
---

# WinHelpCall

!!! abstract "Command &middot; `ComOff.chm`"
    Command: WinHelpCall

Opens a help file with the extension .hlp or .chm.

## Signature

```python
dd.WinHelpCall(WINHelpFile, WinHelpCommand, WinHelpTopic)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the Microsoft Web site for the Microsoft help compiler and for more information on syntax in help calls.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">WINHelpFile</td>
<td>Specifies the name of a help file.<div id="exp_WINHelpFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">WinHelpCommand</td>
<td>Specifies the type of search term.<div id="exp_WinHelpCommand">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpKey"</pre></donottranslate></td>
<td>Help key</td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpContext"</pre></donottranslate></td>
<td>Help context string</td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpCmd"</pre></donottranslate></td>
<td>Command</td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpQuit"</pre></donottranslate></td>
<td>Quit</td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpIndex"</pre></donottranslate></td>
<td>Index</td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpContents"</pre></donottranslate></td>
<td>Contents</td></tr>
<tr><td width="150"><donottranslate><pre>"WINHelpPartKey"</pre></donottranslate></td>
<td>PartialKey</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">WinHelpTopic</td>
<td>Specifies the URL of the help page.<div id="exp_WinHelpTopic">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.WinHelpCall("diadem.chm","WINHelpIndex","WinHelpCall")
```

---

*Source: `ComOff/WinHelpCall.htm`*

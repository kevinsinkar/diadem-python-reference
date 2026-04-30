---
title: "WndShow"
description: "Opens or closes a DIAdem panel."
---

# WndShow

!!! abstract "Command &middot; `ComOff.chm`"
    Command: WndShow

Opens or closes a DIAdem panel.

## Signature

```python
dd.WndShow(WndName, WndMode)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can use the <span class="Monospace">HIDE</span> selection term with the keyword <span class="Monospace">Shell</span> for the <a href="../../../varoff/variables/wndname/">WndName</a> variable. This hides DIAdem. The keyword <span class="Monospace">Show</span> makes DIAdem visible again.<br attr="ext"/>DIAdem does not support the selection term <span class="Monospace">CLOSE</span> anymore.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Maximize the current window before you use the full screen mode.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">WndName</td>
<td>Specifies the name of a DIAdem panel. By default the <span class="Monospace">WndName</span> variable contains the name of the DIAdem panel which was used last.<div id="exp_WndName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"SHELL"</pre></donottranslate></td>
<td>Active panel</td></tr>
<tr><td width="150"><donottranslate><pre>"NAVIGATOR"</pre></donottranslate></td>
<td>DIAdem NAVIGATOR panel</td></tr>
<tr><td width="150"><donottranslate><pre>"REPORT"</pre></donottranslate></td>
<td>DIAdem REPORT panel</td></tr>
<tr><td width="150"><donottranslate><pre>"VIEW"</pre></donottranslate></td>
<td>DIAdem VIEW panel</td></tr>
<tr><td width="150"><donottranslate><pre>"ANALYSIS"</pre></donottranslate></td>
<td>DIAdem ANALYSIS panel</td></tr>
<tr><td width="150"><donottranslate><pre>"DAC"</pre></donottranslate></td>
<td>DIAdem DAC panel</td></tr>
<tr><td width="150"><donottranslate><pre>"VISUAL"</pre></donottranslate></td>
<td>DIAdem VISUAL panel</td></tr>
<tr><td width="150"><donottranslate><pre>"SCRIPT"</pre></donottranslate></td>
<td>DIAdem SCRIPT panel</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">WndMode</td>
<td>Specifies the display mode for a DIAdem panel.<div id="exp_WndMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"OPEN"</pre></donottranslate></td>
<td>Open DIAdem panel</td></tr>
<tr><td width="150"><donottranslate><pre>"CLOSE"</pre></donottranslate></td>
<td>Close DIAdem panel</td></tr>
<tr><td width="150"><donottranslate><pre>"SHOW"</pre></donottranslate></td>
<td>Display DIAdem panel</td></tr>
<tr><td width="150"><donottranslate><pre>"MAXIMIZE"</pre></donottranslate></td>
<td>Maximize DIAdem panel</td></tr>
<tr><td width="150"><donottranslate><pre>"MINIMIZE"</pre></donottranslate></td>
<td>Minimize DIAdem panel</td></tr>
<tr><td width="150"><donottranslate><pre>"NORMAL"</pre></donottranslate></td>
<td>DIAdem panel default size</td></tr>
<tr><td width="150"><donottranslate><pre>"FULLSIZE"</pre></donottranslate></td>
<td>Full screen</td></tr>
<tr><td width="150"><donottranslate><pre>"HIDE"</pre></donottranslate></td>
<td>Hide DIAdem panel</td></tr>
</table>
</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>You only can use the <span class="Monospace">HIDE</span> selection term with the keyword <span class="Monospace">Shell</span> for the <a href="../../../varoff/variables/wndname/">WndName</a> variable. This hides DIAdem. The keyword <span class="Monospace">Show</span> makes DIAdem visible again.<br attr="ext"/>DIAdem does not support the selection term <span class="Monospace">CLOSE</span> anymore.</td></tr></table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.WndShow("VIEW","MAXIMIZE")
dd.WndShow("VIEW","FULLSIZE")
dd.MsgBoxDisp("Press <CTRL-U> to exit fullsize mode")
```

```python
dd.WndShow("SHELL","FULLSIZE")
dd.MsgBoxDisp("Press <CTRL-U> to exit fullsize mode")
```

---

*Source: `ComOff/WndShow.htm`*

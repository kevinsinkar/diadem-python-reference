---
title: "PrinterPaperSizeListGet"
description: "Specifies a list of paper formats that the printer supports. You can use the returned names directly in scripts."
---

# PrinterPaperSizeListGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PrinterPaperSizeListGet

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('PrinterName', ...)   # instead of dd.PrinterName = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Specifies a list of paper formats that the printer supports. You can use the returned names directly in scripts.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note </strong>If you use the DIAdem PDF printer, the last entry in this variable, which describes the port, must be "NUL", for example, "winspool,DIAdem PDF Export,NUL:".</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[PrinterName]</td>
<td>Specifies the name of the enabled printer. If you do not specify the <span class="Monospace">PrinterName</span> variable, DIAdem uses the current default printer.<div id="exp_PrinterName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p>The name <span class="Monospace">PrintName</span> is obsolete. Use <span class="Monospace">PrinterName</span> instead.</p><h2>Example</h2>
<p class="Body">Select interactively the printer you want and specify the variable <span class="Monospace">PrinterName</span>:</p>
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue"><pre><donottranslate><span class="Hldiademvariable">PrinterName</span> = <span class="HlString">"winspool,\\National\LJ5P,Ne02:"</span></donottranslate></pre></div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>dd.PrinterName = <span class="HlString">"winspool,\\\\National\\LJ5P,Ne02:"</span> 
</donottranslate></pre></div>
<p>
</p><table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note </strong>If you use the DIAdem PDF printer, the last entry in this variable, which describes the port, must be "NUL", for example, "winspool,DIAdem PDF Export,NUL:".</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">String variable</a> type.</td></tr>
</table>
</div>

## Python example

```python
dd.PrinterName = "winspool,\\\\National\\LJ5P,Ne02:"
```

---

*Source: `ComOff/PrinterPaperSizeListGet.htm`*

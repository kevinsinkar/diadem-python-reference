---
title: "PrinterPaperSizeGet"
description: "Receives the paper format of the printer."
---

# PrinterPaperSizeGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: PrinterPaperSizeGet

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.TextVarSet('PrinterName', ...)   # instead of dd.PrinterName = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Receives the paper format of the printer.

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
<td>Specifies the paper format. The return value is a PrinterPaperSizes type.<div id="exp_PrinterPaperSizes">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"LETTER"</pre></donottranslate></td>
<td>LETTER</td></tr>
<tr><td width="150"><donottranslate><pre>"LETTERSMALL"</pre></donottranslate></td>
<td>LETTERSMALL</td></tr>
<tr><td width="150"><donottranslate><pre>"TABLOID"</pre></donottranslate></td>
<td>TABLOID</td></tr>
<tr><td width="150"><donottranslate><pre>"LEDGER"</pre></donottranslate></td>
<td>LEDGER</td></tr>
<tr><td width="150"><donottranslate><pre>"LEGAL"</pre></donottranslate></td>
<td>LEGAL</td></tr>
<tr><td width="150"><donottranslate><pre>"STATEMENT"</pre></donottranslate></td>
<td>STATEMENT</td></tr>
<tr><td width="150"><donottranslate><pre>"EXECUTIVE"</pre></donottranslate></td>
<td>EXECUTIVE</td></tr>
<tr><td width="150"><donottranslate><pre>"A3"</pre></donottranslate></td>
<td>A3</td></tr>
<tr><td width="150"><donottranslate><pre>"A4"</pre></donottranslate></td>
<td>A4</td></tr>
<tr><td width="150"><donottranslate><pre>"A4SMALL"</pre></donottranslate></td>
<td>A4SMALL</td></tr>
<tr><td width="150"><donottranslate><pre>"A5"</pre></donottranslate></td>
<td>A5</td></tr>
<tr><td width="150"><donottranslate><pre>"B4"</pre></donottranslate></td>
<td>B4</td></tr>
<tr><td width="150"><donottranslate><pre>"B5"</pre></donottranslate></td>
<td>B5</td></tr>
<tr><td width="150"><donottranslate><pre>"FOLIO"</pre></donottranslate></td>
<td>FOLIO</td></tr>
<tr><td width="150"><donottranslate><pre>"QUARTO"</pre></donottranslate></td>
<td>QUARTO</td></tr>
<tr><td width="150"><donottranslate><pre>"10X14"</pre></donottranslate></td>
<td>10X14</td></tr>
<tr><td width="150"><donottranslate><pre>"11X17"</pre></donottranslate></td>
<td>11X17</td></tr>
<tr><td width="150"><donottranslate><pre>"NOTE"</pre></donottranslate></td>
<td>NOTE</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_9"</pre></donottranslate></td>
<td>ENV_9</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_10"</pre></donottranslate></td>
<td>ENV_10</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_11"</pre></donottranslate></td>
<td>ENV_11</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_12"</pre></donottranslate></td>
<td>ENV_12</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_14"</pre></donottranslate></td>
<td>ENV_14</td></tr>
<tr><td width="150"><donottranslate><pre>"CSHEET"</pre></donottranslate></td>
<td>CSHEET</td></tr>
<tr><td width="150"><donottranslate><pre>"DSHEET"</pre></donottranslate></td>
<td>DSHEET</td></tr>
<tr><td width="150"><donottranslate><pre>"ESHEET"</pre></donottranslate></td>
<td>ESHEET</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_DL"</pre></donottranslate></td>
<td>ENV_DL</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_C5"</pre></donottranslate></td>
<td>ENV_C5</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_C3"</pre></donottranslate></td>
<td>ENV_C3</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_C4"</pre></donottranslate></td>
<td>ENV_C4</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_C6"</pre></donottranslate></td>
<td>ENV_C6</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_C65"</pre></donottranslate></td>
<td>ENV_C65</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_B4"</pre></donottranslate></td>
<td>ENV_B4</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_B5"</pre></donottranslate></td>
<td>ENV_B5</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_B6"</pre></donottranslate></td>
<td>ENV_B6</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_ITALY"</pre></donottranslate></td>
<td>ENV_ITALY</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_MONARCH"</pre></donottranslate></td>
<td>ENV_MONARCH</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_PERSONAL"</pre></donottranslate></td>
<td>ENV_PERSONAL</td></tr>
<tr><td width="150"><donottranslate><pre>"FANFOLD_US"</pre></donottranslate></td>
<td>FANFOLD_US</td></tr>
<tr><td width="150"><donottranslate><pre>"FANFOLD_STD_GERMAN"</pre></donottranslate></td>
<td>FANFOLD_STD_GERMAN</td></tr>
<tr><td width="150"><donottranslate><pre>"FANFOLD_LGL_GERMAN"</pre></donottranslate></td>
<td>FANFOLD_LGL_GERMAN</td></tr>
<tr><td width="150"><donottranslate><pre>"ISO_B4"</pre></donottranslate></td>
<td>ISO_B4</td></tr>
<tr><td width="150"><donottranslate><pre>"JAPANESE_POSTCARD"</pre></donottranslate></td>
<td>JAPANESE_POSTCARD</td></tr>
<tr><td width="150"><donottranslate><pre>"9X11"</pre></donottranslate></td>
<td>9X11</td></tr>
<tr><td width="150"><donottranslate><pre>"10X11"</pre></donottranslate></td>
<td>10X11</td></tr>
<tr><td width="150"><donottranslate><pre>"15X11"</pre></donottranslate></td>
<td>15X11</td></tr>
<tr><td width="150"><donottranslate><pre>"ENV_INVITE"</pre></donottranslate></td>
<td>ENV_INVITE</td></tr>
<tr><td width="150"><donottranslate><pre>"RESERVED_48"</pre></donottranslate></td>
<td>RESERVED_48</td></tr>
<tr><td width="150"><donottranslate><pre>"RESERVED_49"</pre></donottranslate></td>
<td>RESERVED_49</td></tr>
<tr><td width="150"><donottranslate><pre>"LETTER_EXTRA"</pre></donottranslate></td>
<td>LETTER_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"LEGAL_EXTRA"</pre></donottranslate></td>
<td>LEGAL_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"TABLOID_EXTRA"</pre></donottranslate></td>
<td>TABLOID_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"A4_EXTRA"</pre></donottranslate></td>
<td>A4_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"LETTER_TRANSVERSE"</pre></donottranslate></td>
<td>LETTER_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"A4_TRANSVERSE"</pre></donottranslate></td>
<td>A4_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"LETTER_EXTRA_TRANSVERSE"</pre></donottranslate></td>
<td>LETTER_EXTRA_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"A_PLUS"</pre></donottranslate></td>
<td>A_PLUS</td></tr>
<tr><td width="150"><donottranslate><pre>"B_PLUS"</pre></donottranslate></td>
<td>B_PLUS</td></tr>
<tr><td width="150"><donottranslate><pre>"LETTER_PLUS"</pre></donottranslate></td>
<td>LETTER_PLUS</td></tr>
<tr><td width="150"><donottranslate><pre>"A4_PLUS"</pre></donottranslate></td>
<td>A4_PLUS</td></tr>
<tr><td width="150"><donottranslate><pre>"A5_TRANSVERSE"</pre></donottranslate></td>
<td>A5_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"B5_TRANSVERSE"</pre></donottranslate></td>
<td>B5_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"A3_EXTRA"</pre></donottranslate></td>
<td>A3_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"A5_EXTRA"</pre></donottranslate></td>
<td>A5_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"B5_EXTRA"</pre></donottranslate></td>
<td>B5_EXTRA</td></tr>
<tr><td width="150"><donottranslate><pre>"A2"</pre></donottranslate></td>
<td>A2</td></tr>
<tr><td width="150"><donottranslate><pre>"A3_TRANSVERSE"</pre></donottranslate></td>
<td>A3_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"A3_EXTRA_TRANSVERSE"</pre></donottranslate></td>
<td>A3_EXTRA_TRANSVERSE</td></tr>
<tr><td width="150"><donottranslate><pre>"DBL_JAPANESE_POSTCARD"</pre></donottranslate></td>
<td>DBL_JAPANESE_POSTCARD</td></tr>
<tr><td width="150"><donottranslate><pre>"A6"</pre></donottranslate></td>
<td>A6</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_KAKU2"</pre></donottranslate></td>
<td>JENV_KAKU2</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_KAKU3"</pre></donottranslate></td>
<td>JENV_KAKU3</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_CHOU3"</pre></donottranslate></td>
<td>JENV_CHOU3</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_CHOU4"</pre></donottranslate></td>
<td>JENV_CHOU4</td></tr>
<tr><td width="150"><donottranslate><pre>"LETTER_ROTATED"</pre></donottranslate></td>
<td>LETTER_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"A3_ROTATED"</pre></donottranslate></td>
<td>A3_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"A4_ROTATED"</pre></donottranslate></td>
<td>A4_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"A5_ROTATED"</pre></donottranslate></td>
<td>A5_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"B4_JIS_ROTATED"</pre></donottranslate></td>
<td>B4_JIS_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"B5_JIS_ROTATED"</pre></donottranslate></td>
<td>B5_JIS_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"JAPANESE_POSTCARD_ROTATED"</pre></donottranslate></td>
<td>JAPANESE_POSTCARD_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"DBL_JAPANESE_POSTCARD_ROTATED"</pre></donottranslate></td>
<td>DBL_JAPANESE_POSTCARD_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"A6_ROTATED"</pre></donottranslate></td>
<td>A6_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_KAKU2_ROTATED"</pre></donottranslate></td>
<td>JENV_KAKU2_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_KAKU3_ROTATED"</pre></donottranslate></td>
<td>JENV_KAKU3_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_CHOU3_ROTATED"</pre></donottranslate></td>
<td>JENV_CHOU3_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_CHOU4_ROTATED"</pre></donottranslate></td>
<td>JENV_CHOU4_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"B6_JIS"</pre></donottranslate></td>
<td>B6_JIS</td></tr>
<tr><td width="150"><donottranslate><pre>"B6_JIS_ROTATED"</pre></donottranslate></td>
<td>B6_JIS_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"12X11"</pre></donottranslate></td>
<td>12X11</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_YOU4"</pre></donottranslate></td>
<td>JENV_YOU4</td></tr>
<tr><td width="150"><donottranslate><pre>"JENV_YOU4_ROTATED"</pre></donottranslate></td>
<td>JENV_YOU4_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"P16K"</pre></donottranslate></td>
<td>P16K</td></tr>
<tr><td width="150"><donottranslate><pre>"P32K"</pre></donottranslate></td>
<td>P32K</td></tr>
<tr><td width="150"><donottranslate><pre>"P32KBIG"</pre></donottranslate></td>
<td>P32KBIG</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_1"</pre></donottranslate></td>
<td>PENV_1</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_2"</pre></donottranslate></td>
<td>PENV_2</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_3"</pre></donottranslate></td>
<td>PENV_3</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_4"</pre></donottranslate></td>
<td>PENV_4</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_5"</pre></donottranslate></td>
<td>PENV_5</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_6"</pre></donottranslate></td>
<td>PENV_6</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_7"</pre></donottranslate></td>
<td>PENV_7</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_8"</pre></donottranslate></td>
<td>PENV_8</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_9"</pre></donottranslate></td>
<td>PENV_9</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_10"</pre></donottranslate></td>
<td>PENV_10</td></tr>
<tr><td width="150"><donottranslate><pre>"P16K_ROTATED"</pre></donottranslate></td>
<td>P16K_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"P32K_ROTATED"</pre></donottranslate></td>
<td>P32K_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"P32KBIG_ROTATED"</pre></donottranslate></td>
<td>P32KBIG_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_1_ROTATED"</pre></donottranslate></td>
<td>PENV_1_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_2_ROTATED"</pre></donottranslate></td>
<td>PENV_2_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_3_ROTATED"</pre></donottranslate></td>
<td>PENV_3_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_4_ROTATED"</pre></donottranslate></td>
<td>PENV_4_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_5_ROTATED"</pre></donottranslate></td>
<td>PENV_5_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_6_ROTATED"</pre></donottranslate></td>
<td>PENV_6_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_7_ROTATED"</pre></donottranslate></td>
<td>PENV_7_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_8_ROTATED"</pre></donottranslate></td>
<td>PENV_8_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_9_ROTATED"</pre></donottranslate></td>
<td>PENV_9_ROTATED</td></tr>
<tr><td width="150"><donottranslate><pre>"PENV_10_ROTATED"</pre></donottranslate></td>
<td>PENV_10_ROTATED</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.PrinterName = "winspool,\\\\National\\LJ5P,Ne02:"
```

---

*Source: `ComOff/PrinterPaperSizeGet.htm`*

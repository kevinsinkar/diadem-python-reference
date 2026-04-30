---
title: "TextFileEncoding"
description: "Specifies the character encoding of a file. The function uses the Byte Order Mark (BOM) of the file to specify the character encoding."
---

# TextFileEncoding

!!! abstract "Command &middot; `ComOff.chm`"
    Command: TextFileEncoding

Specifies the character encoding of a file. The function uses the Byte Order Mark (BOM) of the file to specify the character encoding.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">FileName</td>
<td>Specifies the filename.<div id="exp_FileName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String</a></td></tr>
<tr>
<td>Maximum <a href="../../../varoff/variables/applicationmaxpathlength/">ApplicationMaxPathLength</a> characters<br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In many commands, you can use the <span class="Monospace">*</span> wildcard for any number of characters, and the <span class="Monospace">?</span> wildcard for one character.</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is an <a href="#" data-unresolved="1">Integer variable</a> type. Contains the character encoding<table class="Borderless">
<tr>
<td width="30">4</td>
<td width="150"><span class="Monospace">eTextFileAttributeANSI</span></td>
<td>Encoded in ANSI.</td>
</tr>
<tr>
<td width="30">8</td>
<td width="150"><span class="Monospace">eTextFileAttributeUnicode</span></td>
<td>Encoded in Unicode.</td>
</tr>
<tr>
<td width="30">16</td>
<td width="150"><span class="Monospace">eTextFileAttributeUTF8</span></td>
<td>Encoded in UTF8.</td>
</tr>
</table><!-- Start --><h2>Examples</h2>
<p class="Body">The following example specifies the character encoding of a file:</p>
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue">
<pre><donottranslate><span class="HlVBSKeyword">Dim</span> intMyEncode
intMyEncode = <span class="Hldiademcommand">TextFileEncoding</span>(<span class="Hldiademvariable">ScriptReadPath</span> &amp; <span class="HlString">"NewText.txt"</span>)
<span class="HlVBSKeyword">Select</span> <span class="HlVBSKeyword">Case</span> intMyEncode
<span class="HlVBSKeyword">Case</span> <span class="Hldiademconstant">eTextFileAttributeANSI</span>
  <span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">MsgBoxDisp</span>(<span class="HlString">"ANSI"</span>)
<span class="HlVBSKeyword">Case</span> <span class="Hldiademconstant">eTextFileAttributeUnicode</span>
  <span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">MsgBoxDisp</span>(<span class="HlString">"Unicode"</span>)
<span class="HlVBSKeyword">Case</span> <span class="Hldiademconstant">eTextFileAttributeUTF8</span>
  <span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">MsgBoxDisp</span>(<span class="HlString">"UTF8"</span>)
<span class="HlVBSKeyword">Case</span> <span class="HlVBSKeyword">Else</span>
  <span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">MsgBoxDisp</span>(<span class="HlString">"Error occured"</span>)
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Select</span></donottranslate></pre>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate>intMyEncode = dd.TextFileEncoding(dd.ScriptReadPath + <span class="HlString">"NewText.txt"</span>) 
select_variable_0 = intMyEncode 
<span class="HlVBSKeyword">if</span> (select_variable_0 == dd.eTextFileAttributeANSI) : 
    dd.MsgBoxDisp(<span class="HlString">"ANSI"</span>) 
<span class="HlVBSKeyword">elif</span> (select_variable_0 == dd.eTextFileAttributeUnicode) : 
    dd.MsgBoxDisp(<span class="HlString">"Unicode"</span>) 
<span class="HlVBSKeyword">elif</span> (select_variable_0 == dd.eTextFileAttributeUTF8) : 
    dd.MsgBoxDisp(<span class="HlString">"UTF8"</span>) 
<span class="HlVBSKeyword">else</span>: 
    dd.MsgBoxDisp(<span class="HlString">"Error occured"</span>) 
</donottranslate></pre></div>
<h2>Related Functions</h2><p class="Body"><a href="../textfileeol/">Command: TextFileEOL</a> | <a href="#" data-unresolved="1">Function: FR</a> | <a href="#" data-unresolved="1">Function: TextFileEOF</a> | <a href="#" data-unresolved="1">Function: TextFileError</a> | <a href="#" data-unresolved="1">Function: TextFileErrorTxt</a> | <a href="#" data-unresolved="1">Function: TextFileSeek</a></p><!-- End --></td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eTextFileAttributeANSI` | 4 | Encoded in ANSI. |
| `eTextFileAttributeUnicode` | 8 | Encoded in Unicode. |
| `eTextFileAttributeUTF8` | 16 | Encoded in UTF8. |

## Python example

```python
intMyEncode = dd.TextFileEncoding(dd.ScriptReadPath + "NewText.txt")
select_variable_0 = intMyEncode
if (select_variable_0 == dd.eTextFileAttributeANSI) :
    dd.MsgBoxDisp("ANSI")
elif (select_variable_0 == dd.eTextFileAttributeUnicode) :
    dd.MsgBoxDisp("Unicode")
elif (select_variable_0 == dd.eTextFileAttributeUTF8) :
    dd.MsgBoxDisp("UTF8")
else:
    dd.MsgBoxDisp("Error occured")
```

---

*Source: `ComOff/TextFileEncoding.htm`*

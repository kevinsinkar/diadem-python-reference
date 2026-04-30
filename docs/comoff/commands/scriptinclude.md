---
title: "ScriptInclude"
description: "Integrates a script in another script."
---

# ScriptInclude

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ScriptInclude

Integrates a script in another script.

## Signature

```python
dd.ScriptInclude(ScriptFile, [ScriptScope])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Call the <span class="Monospace">ScriptInclude</span> command only once at the beginning of a script for each script to be included. Do not call the <span class="Monospace">ScriptInclude</span> command in loops. The following table describes when to use the <a href="../scriptstart/">ScriptStart</a> command instead of the <span class="Monospace">ScriptInclude</span> command. If you use the <span class="Monospace">ScriptInclude</span> command instead of the <span class="Monospace">ScriptStart</span> command you can <a href="#" data-unresolved="1">speed up scripts</a>.<table class="Borderless">
<tr>
<td><strong>ScriptStart</strong></td>
<td><strong>ScriptInclude</strong></td><td> </td>
</tr>
<tr>
<td> </td>
<td>X</td><td>When you use transfer parameters</td>
</tr>
<tr>
<td> </td>
<td>X</td><td>When you use return values</td>
</tr>
<tr>
<td> </td>
<td>X</td>
<td>When you debug calls in another script</td>
</tr>
<tr>
<td> </td>
<td>X</td>
<td>When you use name spaces</td>
</tr>
<tr>
<td> </td>
<td>X</td>
<td>When you use objects and variables from another script</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you start a script as program parameter</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you specify menus, buttons, and other controls to start a script</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you call scripts via OLE</td>
</tr>
<tr>
<td>X</td>
<td> </td>
<td>When you cancel the started script or local error for this script</td>
</tr>
</table>
</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ScriptFile</td>
<td>Specifies the name of a script file.<div id="exp_ScriptFile">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ScriptScope]</td>
<td>Specifies the name space of a script. By default the <span class="Monospace">ScriptCode</span> variable contains an empty text.<div id="exp_ScriptScope">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 255 characters</td></tr>
</table>
<p class="Body">Use the name space to distinguish between procedures that have the same names, in different script files.</p>
<h2>Example</h2>
<p class="Body">The following example assumes that the <span class="Monospace">MyFunc</span> function is in the <span class="Monospace">Test.vbs</span> script as well as the <span class="Monospace">MyLib.vbs</span> script. You can use the name space to distinguish between the two functions. In the example, the <span class="Monospace">MyResult</span> variable receives the result of the <span class="Monospace">MyFunc</span> function in the <span class="Monospace">Test.vbs</span> file and the <span class="Monospace">MyOtherResult</span> variable receives the result of the <span class="Monospace">MyFunc</span> function in the <span class="Monospace">MyLib.vbs</span> file. </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue"><pre><donottranslate><span class="HlVBSKeyword">Dim</span> MyResult
<span class="HlVBSKeyword">Dim</span> MyOtherResult
<span class="Hldiademvariable">ScriptScope</span> = <span class="HlString">"Test"</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">ScriptInclude</span>(<span class="HlString">"Test.vbs"</span>,<span class="Hldiademvariable">ScriptScope</span>)
<span class="Hldiademvariable">ScriptScope</span> = <span class="HlString">"GlobalLib"</span>
<span class="HlVBSKeyword">Call</span> <span class="Hldiademcommand">ScriptInclude</span>(<span class="HlString">"MyLib.vbs"</span>,<span class="Hldiademvariable">ScriptScope</span>)
MyResult = Test.MyFunc
MyOtherResult = GlobalLib.MyFunc</donottranslate></pre></div>
</div></td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
ScriptScope = "Test"
ScriptInclude("Test.vbs",ScriptScope)
ScriptScope = "GlobalLib"
ScriptInclude("MyLib.vbs",ScriptScope)
MyResult = Test.MyFunc
MyOtherResult = GlobalLib.MyFunc
```

```python
# Register all functions and procedures of Function_Library.vbs
ScriptInclude("Function_Library")
# Calling the function
GetChnName(1)
MsgBoxDisp(strChannelName)
GetChnName(5)
MsgBoxDisp(strChannelName)
```

```python
# Labelling as subscript
Subsequence()
# Initialization
# Procedure for evaluating a channel name
def GetChnName(intChannelNo):
    strChannelName ="<Channel does not exist!>" ' Initialize string
    if intChannelNo <= GlobUsedCHn:
        ' Less then maximum channel number
    strChannelName = ChnName(intChannelNo)
```

---

*Source: `ComOff/ScriptInclude.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

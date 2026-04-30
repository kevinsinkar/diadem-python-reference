---
title: "HSLtoRGB"
description: "Converts a color value from the HSL model (Hue, Saturation, Luminosity) into the RGB model (Red, Green, Blue)."
---

# HSLtoRGB

!!! abstract "Command &middot; `ComOff.chm`"
    Command: HSLtoRGB

Converts a color value from the HSL model (Hue, Saturation, Luminosity) into the RGB model (Red, Green, Blue).

## Notes

<div markdown="1">
<table class="Borderless" id="table1">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td>
<td><strong>Note  </strong>Use the following function to calculate the HSL color value from the individual color parts.<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue"><pre><donottranslate><code><span class="HlVBSKeyword">Function</span> HSL(HValue, SValue, LValue)
  HSL = <span class="HlVBSKeyword">CLng</span>(HValue+ (SValue* <span class="HlNumbers">256</span>) + (LValue * <span class="HlNumbers">65536</span>))
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Function</span></code></donottranslate></pre></div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate><span class="HlVBSKeyword">def</span> HSL(HValue, SValue, LValue): 
    HSL = <span class="HlVBSKeyword">int</span>(HValue+ (SValue* <span class="HlNumbers">256</span>) + (LValue * <span class="HlNumbers">65536</span>)) 
    <span class="HlVBSKeyword">return</span> HSL</donottranslate></pre></div></td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">HSLValue</td>
<td>Specifies the HSL color value.<div id="exp_HSLValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the RGB values as a <a href="#" data-unresolved="1">Longinteger variable</a>.</td></tr>
</table>
</div>

## Python example

```python
def HSL(HValue, SValue, LValue):
    HSL = int(HValue+ (SValue* 256) + (LValue * 65536))
    return HSL
```

---

*Source: `ComOff/HSLtoRGB.htm`*

---
title: "ChnClassXRedXY"
description: "Classifies a signal and reduces the result data."
---

# ChnClassXRedXY

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnClassXRedXY

!!! warning "Read-only on `DIAdem.TOCmd` &mdash; use the bridge"
    The example assigns to a DIAdem global script variable that the
    TOCmd dispatch surfaces as **read-only**. From external Python,
    use the `DIAdem.TOCommand` bridge to set it instead:

    ```python
    bridge = win32com.client.Dispatch("DIAdem.TOCommand")
    bridge.IntegerVarSet('ClassNo', ...)   # instead of dd.ClassNo = ...
    ```

    See [Runtime gotchas &raquo; Some global script variables are read-only](../../getting-started.md#4-some-global-script-variables-are-read-only-on-tocmd) for the full pattern.

Classifies a signal and reduces the result data.

## Signature

```python
dd.ChnClassXRedXY(CALCXChn, ClassChn, CALCYChn, ClassMeth1, ClassXRed, [ChnCRedIP], [ClassDontUseNV], [ClassNVReplace])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Because the channel contains the class limits, the number of channel values must be one value higher than the number of classes. This function does not work with open class limits, so the first value of the channel contains the lowest class limit and the last value contains the highest class limit. The first class contains the values between the first and the second value, the second class contains the values between te second and the third value, and so on.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To include all the values of a function in the classification, the bottom limit value of the first class interval must be smaller than the smallest value of the function you want to classify.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To include all the values of a function in the classification, the top limit value of the last class interval must be greater than the largest value of the function you want to classify.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Because the channel contains the class limits, the number of channel values must be one value higher than the number of classes.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">CALCXChn</td>
<td>Specifies the data channel containing the x-values of the signal.<div id="exp_CALCXChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ClassChn</td>
<td>Specifies which data channel defines the non equidistant class limits.<div id="exp_ClassChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Because the channel contains the class limits, the number of channel values must be one value higher than the number of classes. This function does not work with open class limits, so the first value of the channel contains the lowest class limit and the last value contains the highest class limit. The first class contains the values between the first and the second value, the second class contains the values between te second and the third value, and so on.</td></tr></table>
</div></td></tr>
<tr><td width="150">CALCYChn</td>
<td>Specifies the data channels containing the y-values of the signal.<div id="exp_CALCYChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">ClassMeth1</td>
<td>Specifies how DIAdem specifies the class limits.<div id="exp_ClassMeth1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginEnd"</pre></donottranslate></td>
<td>Number/Begin/End</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginWidth"</pre></donottranslate></td>
<td>Number/Begin/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"NoBeginRange"</pre></donottranslate></td>
<td>Number/Begin/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"NoEndWidth"</pre></donottranslate></td>
<td>Number/End/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"NoEndRange"</pre></donottranslate></td>
<td>Number/End/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"BeginEndWidth"</pre></donottranslate></td>
<td>Begin/End/Width</td></tr>
<tr><td width="150"><donottranslate><pre>"BeginWidthRange"</pre></donottranslate></td>
<td>Begin/Width/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"EndWidthRange"</pre></donottranslate></td>
<td>End/Width/Range</td></tr>
<tr><td width="150"><donottranslate><pre>"Channel"</pre></donottranslate></td>
<td>Channel</td></tr>
</table>
</td></tr>
</table>
<p class="Body">When you use the <span class="Monospace">Automatic</span> method, you specify the number of classes. DIAdem calculates the missing parameters from the maximum and minimum values of the channel to be classified. If you use the <span class="Monospace">Channel</span> method, DIAdem uses the values of the specified channel as class limits.</p>
</div></td></tr>
<tr><td width="150">ClassXRed</td>
<td>Specifies the type of data reduction.<div id="exp_ClassXRed">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Mean"</pre></donottranslate></td>
<td>Mean value</td></tr>
<tr><td width="150"><donottranslate><pre>"minimum"</pre></donottranslate></td>
<td>Minimum</td></tr>
<tr><td width="150"><donottranslate><pre>"maximum"</pre></donottranslate></td>
<td>Maximum</td></tr>
<tr><td width="150"><donottranslate><pre>"Sum"</pre></donottranslate></td>
<td>Sum</td></tr>
<tr><td width="150"><donottranslate><pre>"Quantity"</pre></donottranslate></td>
<td>Number of</td></tr>
</table>
</td></tr>
</table><strong><p class="Body">Valid settings</p></strong><table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" id="AutoNumber1" style="border-collapse: collapse" width="619">
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">Mean</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem averages the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">minimum</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem averages the minimum of all the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">maximum</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem averages the maximum of all the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">Sum</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem totals all the y-values of a class.</p>
</td>
</tr>
<tr>
<td width="87">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt"><span class="Monospace">Quantity</span></p>
</td>
<td width="520">
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">DIAdem specifies the number of y-values of a class.</p>
</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnCRedIP]</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result values of the reducing classification. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not overwrite the input channels.<div id="exp_ChnCRedIP">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ClassDontUseNV]</td>
<td>Specifies whether DIAdem ignores or replaces <a href="../../../varoff/variables/nv/">NoValues</a> in a reducing classification. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not replace NoValues.<div id="exp_ClassDontUseNV">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ClassNVReplace]</td>
<td>Specifies the value with which DIAdem replaces NoValues in a reducing classification. The default value of the <span class="Monospace">ClassNVReplace</span> variable is <span class="Monospace">0</span>.<div id="exp_ClassNVReplace">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ClassNo          = 10
dd.ChnClassXRedXY("[1]/X_Values",None ,"[1]/Y_Values","Automatic","Mean",0,0,0)
```

```python
def CreateClassLimitsChannel(aClassLimits):
    oGroupChns = dd.Data.Root.ChannelGroups(1).Channels
    if not oGroupChns.Exists("ClassLimits") :
        oMyChn = oGroupChns.Add("ClassLimits",dd.DataTypeChnFloat64)
    else:
        oMyChn = oGroupChns("ClassLimits")
    for i in range( 0, len(aClassLimits)-1):
        oMyChn.Values[i+1] = aClassLimits(i)

aValues = [0,1,3,6,10]
CreateClassLimitsChannel(aValues)

dd.ChnClassXRedXY("[1]/X_Values","[1]/ClassLimits","[1]/Y_Values","Channel","Mean",0,0,0)
```

---

*Source: `ComOff/ChnClassXRedXY.htm`*

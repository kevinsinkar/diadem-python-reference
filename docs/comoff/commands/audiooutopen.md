---
title: "AudioOutOpen"
description: "Starts the audio output of channels. For each audio output you receive as the return value a handle with which you end the audio output via the command AudioOut"
---

# AudioOutOpen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: AudioOutOpen

Starts the audio output of channels. For each audio output you receive as the return value a handle with which you end the audio output via the command AudioOutClose .

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Typical sampling rates are between 11 and 96 kHz. However not all sound boards support all sampling rates. Sound boards usually support at least the CD standard of 44.1 kHz.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>To prevent the audio output from slowing down, do not use commands in the user command that take a long time. Do not display message boxes or call other audio commands either.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>In order to output an audio signal, the channel must be completely accessible in the computer memory and not just registered.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>If the <span class="Monospace">AudioBuffersize</span> value is too small, the audio output might have audible interruptions. If the value is too large, the <span class="Monospace">AudioBufferFillEvent</span> user command is rarely used. Additionally the end of an audio output is delayed because DIAdem always outputs the complete buffer.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>DIAdem continues the script directly after calling the <span class="Monospace">AudioOutOpen</span> command. Use the <a href="../audiooutwaituntilend/">AudioOutWaitUntilEnd</a> command to interrupt the script during the audio output.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">AudioLeftChn</td>
<td>Specifies the left channel for the audio output.<div id="exp_AudioLeftChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[AudioRightChn]</td>
<td>Specifies the right channel for the audio output. If you do not specify a channel, DIAdem uses the left channel.<div id="exp_AudioRightChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[AudioStartRow]</td>
<td>Specifies the first channel row from where DIAdem starts the audio output. If you do not specify a value or if you specify a negative value, DIAdem uses the first value of the channel.<div id="exp_AudioStartRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioStartRow &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[AudioEndRow]</td>
<td>Specifies the last channel row at which DIAdem ends the audio output. If you do not specify a value, if you specify a negative value, or if you specify a value larger than the channel length, DIAdem uses the last channel value.<div id="exp_AudioEndRow">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioEndRow &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[AudioSampleRate]</td>
<td>Specifies in Hz the sampling rate DIAdem uses to generate audio signals. If you specify <span class="Monospace">0</span> or no value, DIAdem tries to specify the sampling rate from the properties <span class="Monospace">wf_xunit_string</span> and <span class="Monospace">wf_increment</span>. If these properties are missing or in an incorrect unit, DIAdem uses the value 44.1 kHz.<div id="exp_AudioSampleRate">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioSampleRate &lt;= 96000</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Typical sampling rates are between 11 and 96 kHz. However not all sound boards support all sampling rates. Sound boards usually support at least the CD standard of 44.1 kHz.</td></tr></table>
</div></td></tr>
<tr><td width="150">[AudioAutoRepeat]</td>
<td>Specifies whether DIAdem restarts the audio output automatically at the end. If the value is <span class="Monospace">TRUE</span>, DIAdem starts the audio output automatically.<div id="exp_AudioAutoRepeat">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[AudioStartSuspended]</td>
<td>Specifies that the audio output does not start directly. Use the commands <a href="../audiooutsuspend/">AudioOutSuspend</a> and <a href="../audiooutresume/">AudioOutResume</a> to stop or to continue the audio output.<div id="exp_AudioStartSuspended">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[AudioBufferFillEvent]</td>
<td>Specifies the user command that DIAdem calls when loading new data to the clipboard of the audio output.<div id="exp_AudioBufferFillEvent">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
<p>The user command has the following structure:</p>
<table align="left" cellspacing="1"><tr><td class="vbstab"><a>VBScript</a></td><td class="pytab"><a>Python</a></td> </tr></table><p> </p>
<div class="copyblue"><p class="body"><a href="#">Copy script</a></p></div>
<div class="codeblue"><donottranslate><pre><span class="HlVBSKeyword">Sub</span> MyAudioOutCallback(<span class="Hldiademvariable">AudioHandle</span>, CurrentIndex, BlockSize, SampleRate, MaxIndex)
  <span class="HlComment">Rem Some commands</span>
<span class="HlVBSKeyword">End</span> <span class="HlVBSKeyword">Sub</span></pre></donottranslate>
</div><div class="copyyellow"><p class="body"><a href="#">Copy script</a></p></div><div class="codeyellow"><pre><donottranslate><span class="HlVBSKeyword">def</span> MyAudioOutCallback(<span class="Hldiademvariable">AudioHandle</span>, CurrentIndex, BlockSize, SampleRate, MaxIndex): 
    <span class="HlVBSKeyword">pass</span> <span class="HlComment"># Some commands </span>
</donottranslate></pre></div>
<h2>Input Parameters</h2>
<table class="Borderless">
<tr><td width="150">AudioHandle</td>
<td>Specifies the handle of the audio output.</td></tr>
<tr><td width="150">CurrentIndex</td>
<td>Specifies which row of the channel DIAdem uses for filling the workspace.</td></tr>
<tr><td width="150">BlockSize</td>
<td>Specifies the number of values DIAdem uses for the buffer of the audio output.</td></tr>
<tr><td width="150">SampleRate</td>
<td>Specifies in Hz the sampling rate DIAdem uses to generate audio signals.</td></tr>
<tr><td width="150">MaxIndex</td>
<td>Specifies the maximum row index that corresponds to the minimum of both channel lengths.</td></tr>
</table>
<p>At the end of the audio output DIAdem calls the user command with the following values: <span class="Monospace">CurrentIndex = -1</span>, <span class="Monospace">BlockSize = 0</span>, <span class="Monospace">SampleRate = 0</span>, and <span class="Monospace">MaxIndex = -1</span>.</p>
<p></p><table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>To prevent the audio output from slowing down, do not use commands in the user command that take a long time. Do not display message boxes or call other audio commands either.</td></tr></table>
 

	
</div></td></tr>
<tr><td width="150">[AudioBuffersize]</td>
<td>Specifies the number of values DIAdem uses for the buffer of the audio output. If you do not specify this value, DIAdem specifies the size of the buffer automatically.<div id="exp_AudioBuffersize">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= AudioBuffersize &lt;= 1000000</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies the handle of the audio output. The return value is a AudioHandle type.<div id="exp_AudioHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>-2147483648 &lt;= AudioHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
def MyAudioOutCallback(AudioHandle, CurrentIndex, BlockSize, SampleRate, MaxIndex):
    pass # Some commands
```

```python
iHandle= dd.AudioOutOpen(dd.Data.Root.ChannelGroups(2).Channels("Noise_1"),dd.Data.Root.ChannelGroups(2).Channels("Noise_2"))
```

---

*Source: `ComOff/AudioOutOpen.htm`*

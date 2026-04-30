---
title: "OnFilterKeyShortcut"
description: "Specifies the user function DIAdem executes when you press <Shift>, <Ctrl>, or <Alt> button combinations. DIAdem does not execute this function when you execute"
---

# OnFilterKeyShortcut

!!! abstract "Variable &middot; `VarOff.chm`"
    Variable: OnFilterKeyShortcut

Specifies the user function DIAdem executes when you press <Shift>, <Ctrl>, or <Alt> button combinations. DIAdem does not execute this function when you execute the shortcut in DIAdem SCRIPT. You cannot assign several user commands to the OnFilterKeyShortcut event.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong>  To test the example script, you must first save the script and register the script as a user command in the dialog box that opens when you select <strong>Settings»Extensions»User Commands</strong>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">Panel</td>
<td>Specifies the name of the panel in which the shortcut is executed.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Variant variable</a></td>
</tr>
</table>
</td></tr>
<tr><td width="150">KeyCode</td>
<td>Specifies which key is pressed together with the keys &lt;Shift&gt;, &lt;Ctrl&gt; or &lt;Alt&gt;. For a list of possible constants click <a href="#">here</a>:<div id="exp_O2">
<table class="Borderless"><tr><td>8</td><td width="150"><span class="Monospace">KeyCode_BACK</span></td>
<td>Constant for the <span class="Monospace">Back</span> key.</td></tr>
<tr><td>9</td><td width="150"><span class="Monospace">KeyCode_TAB</span></td>
<td>Constant for the <span class="Monospace">Tab</span> key.</td></tr>
<tr><td>13</td><td width="150"><span class="Monospace">KeyCode_RETURN</span></td>
<td>Constant for the <span class="Monospace">Return</span> key.</td></tr>
<tr><td>19</td><td width="150"><span class="Monospace">KeyCode_PAUSE</span></td>
<td>Constant for the <span class="Monospace">Pause</span> key.</td></tr>
<tr><td>20</td><td width="150"><span class="Monospace">KeyCode_CAPITAL</span></td>
<td>Constant for the <span class="Monospace">CapsLock</span> key.</td></tr>
<tr><td>32</td><td width="150"><span class="Monospace">KeyCode_SPACE</span></td>
<td>Constant for the spacebar.</td></tr>
<tr><td>33</td><td width="150"><span class="Monospace">KeyCode_PRIOR</span></td>
<td>Constant for the <span class="Monospace">Page Up</span> key.</td></tr>
<tr><td>34</td><td width="150"><span class="Monospace">KeyCode_NEXT</span></td>
<td>Constant for the <span class="Monospace">Page Down</span> key.</td></tr>
<tr><td>35</td><td width="150"><span class="Monospace">KeyCode_END</span></td>
<td>Constant for the <span class="Monospace">End</span> key.</td></tr>
<tr><td>36</td><td width="150"><span class="Monospace">KeyCode_HOME</span></td>
<td>Constant for the <span class="Monospace">Pos1</span> key.</td></tr>
<tr><td>37</td><td width="150"><span class="Monospace">KeyCode_LEFT</span></td>
<td>Constant for the <span class="Monospace">Left Arrow</span> key.</td></tr>
<tr><td>38</td><td width="150"><span class="Monospace">KeyCode_UP</span></td>
<td>Constant for the <span class="Monospace">Up Arrow</span> key.</td></tr>
<tr><td>39</td><td width="150"><span class="Monospace">KeyCode_RIGHT</span></td>
<td>Constant for the <span class="Monospace">Right Arrow</span> key.</td></tr>
<tr><td>40</td><td width="150"><span class="Monospace">KeyCode_DOWN</span></td>
<td>Constant for the <span class="Monospace">Down Arrow</span> key.</td></tr>
<tr><td>42</td><td width="150"><span class="Monospace">KeyCode_PRINT</span></td>
<td>Constant for the <span class="Monospace">Print</span> key.</td></tr>
<tr><td>45</td><td width="150"><span class="Monospace">KeyCode_INSERT</span></td>
<td>Constant for the <span class="Monospace">Insert</span> key.</td></tr>
<tr><td>46</td><td width="150"><span class="Monospace">KeyCode_DELETE</span></td>
<td>Constant for the <span class="Monospace">Delete</span> key.</td></tr>
<tr><td>47</td><td width="150"><span class="Monospace">KeyCode_HELP</span></td>
<td>Constant for the <span class="Monospace">Help</span> key.</td></tr>
<tr><td>48</td><td width="150"><span class="Monospace">KeyCode_0Key</span></td>
<td>Constant for the <span class="Monospace">0</span> key.</td></tr>
<tr><td>49</td><td width="150"><span class="Monospace">KeyCode_1Key</span></td>
<td>Constant for the <span class="Monospace">1</span> key.</td></tr>
<tr><td>50</td><td width="150"><span class="Monospace">KeyCode_2Key</span></td>
<td>Constant for the <span class="Monospace">2</span> key.</td></tr>
<tr><td>51</td><td width="150"><span class="Monospace">KeyCode_3Key</span></td>
<td>Constant for the <span class="Monospace">3</span> key.</td></tr>
<tr><td>52</td><td width="150"><span class="Monospace">KeyCode_4Key</span></td>
<td>Constant for the <span class="Monospace">4</span> key.</td></tr>
<tr><td>53</td><td width="150"><span class="Monospace">KeyCode_5Key</span></td>
<td>Constant for the <span class="Monospace">5</span> key.</td></tr>
<tr><td>54</td><td width="150"><span class="Monospace">KeyCode_6Key</span></td>
<td>Constant for the <span class="Monospace">6</span> key.</td></tr>
<tr><td>55</td><td width="150"><span class="Monospace">KeyCode_7Key</span></td>
<td>Constant for the <span class="Monospace">7</span> key.</td></tr>
<tr><td>56</td><td width="150"><span class="Monospace">KeyCode_8Key</span></td>
<td>Constant for the <span class="Monospace">8</span> key.</td></tr>
<tr><td>57</td><td width="150"><span class="Monospace">KeyCode_9Key</span></td>
<td>Constant for the <span class="Monospace">9</span> key.</td></tr>
<tr><td>65</td><td width="150"><span class="Monospace">KeyCode_AKey</span></td>
<td>Constant for the <span class="Monospace">A</span> key.</td></tr>
<tr><td>66 to 89</td><td width="150"><span class="Monospace">KeyCode_BKey</span> to <span class="Monospace">KeyCode_YKey</span></td><td>Constant for keys <span class="Monospace">B</span> to <span class="Monospace">Y</span>.</td></tr>
<tr><td>90</td><td width="150"><span class="Monospace">KeyCode_ZKey</span></td>
<td>Constant for the <span class="Monospace">Z</span> key.</td></tr>
<tr><td>91</td><td width="150"><span class="Monospace">KeyCode_LWIN</span></td>
<td>Constant for the left Windows key (Microsoft keyboard)</td></tr>
<tr><td>92</td><td width="150"><span class="Monospace">KeyCode_RWIN</span></td>
<td>Constant for the right Windows key (Microsoft keyboard)</td></tr>
<tr><td>95</td><td width="150"><span class="Monospace">KeyCode_SLEEP</span></td>
<td>Constant for the <span class="Monospace">Sleep</span> key.</td></tr>
<tr><td>96</td><td width="150"><span class="Monospace">KeyCode_NUMPAD0</span></td>
<td>Constant for the <span class="Monospace">0</span> key on the numeric block.</td></tr>
<tr><td>97</td><td width="150"><span class="Monospace">KeyCode_NUMPAD1</span></td>
<td>Constant for the <span class="Monospace">1</span> key on the numeric block.</td></tr>
<tr><td>98</td><td width="150"><span class="Monospace">KeyCode_NUMPAD2</span></td>
<td>Constant for the <span class="Monospace">2</span> key on the numeric block.</td></tr>
<tr><td>99</td><td width="150"><span class="Monospace">KeyCode_NUMPAD3</span></td>
<td>Constant for the <span class="Monospace">3</span> key on the numeric block.</td></tr>
<tr><td>100</td><td width="150"><span class="Monospace">KeyCode_NUMPAD4</span></td>
<td>Constant for the <span class="Monospace">4</span> key on the numeric block.</td></tr>
<tr><td>101</td><td width="150"><span class="Monospace">KeyCode_NUMPAD5</span></td>
<td>Constant for the <span class="Monospace">5</span> key on the numeric block.</td></tr>
<tr><td>102</td><td width="150"><span class="Monospace">KeyCode_NUMPAD6</span></td>
<td>Constant for the <span class="Monospace">6</span> key on the numeric block.</td></tr>
<tr><td>103</td><td width="150"><span class="Monospace">KeyCode_NUMPAD7</span></td>
<td>Constant for the <span class="Monospace">7</span> key on the numeric block.</td></tr>
<tr><td>104</td><td width="150"><span class="Monospace">KeyCode_NUMPAD8</span></td>
<td>Constant for the <span class="Monospace">8</span> key on the numeric block.</td></tr>
<tr><td>105</td><td width="150"><span class="Monospace">KeyCode_NUMPAD9</span></td>
<td>Constant for the <span class="Monospace">9</span> key on the numeric block.</td></tr>
<tr><td>106</td><td width="150"><span class="Monospace">KeyCode_MULTIPLY</span></td>
<td>Constant for the <span class="Monospace">*</span> key on the numeric block.</td></tr>
<tr><td>107</td><td width="150"><span class="Monospace">KeyCode_ADD</span></td>
<td>Constant for the <span class="Monospace">+</span> key on the numeric block.</td></tr>
<tr><td>108</td><td width="150"><span class="Monospace">KeyCode_SEPARATOR</span></td>
<td>Constant for the <span class="Monospace">Separator</span> key on the numeric block.</td></tr>
<tr><td>109</td><td width="150"><span class="Monospace">KeyCode_SUBTRACT</span></td>
<td>Constant for the <span class="Monospace">-</span> key on the numeric block.</td></tr>
<tr><td>110</td><td width="150"><span class="Monospace">KeyCode_DECIMAL</span></td>
<td>Constant for the decimal separator key on the numeric block.</td></tr>
<tr><td>111</td><td width="150"><span class="Monospace">KeyCode_DIVIDE</span></td>
<td>Constant for the ÷ key on the numeric block.</td></tr>
<tr><td>112</td><td width="150"><span class="Monospace">KeyCode_F1</span></td>
<td>Constant for the <span class="Monospace">F1</span> key.</td></tr>
<tr><td>113</td><td width="150"><span class="Monospace">KeyCode_F2</span></td>
<td>Constant for the <span class="Monospace">F2</span> key.</td></tr>
<tr><td>114</td><td width="150"><span class="Monospace">KeyCode_F3</span></td>
<td>Constant for the <span class="Monospace">F3</span> key.</td></tr>
<tr><td>115</td><td width="150"><span class="Monospace">KeyCode_F4</span></td>
<td>Constant for the <span class="Monospace">F4</span> key.</td></tr>
<tr><td>116</td><td width="150"><span class="Monospace">KeyCode_F5</span></td>
<td>Constant for the <span class="Monospace">F5</span> key.</td></tr>
<tr><td>117</td><td width="150"><span class="Monospace">KeyCode_F6</span></td>
<td>Constant for the <span class="Monospace">F6</span> key.</td></tr>
<tr><td>118</td><td width="150"><span class="Monospace">KeyCode_F7</span></td>
<td>Constant for the <span class="Monospace">F7</span> key.</td></tr>
<tr><td>119</td><td width="150"><span class="Monospace">KeyCode_F8</span></td>
<td>Constant for the <span class="Monospace">F8</span> key.</td></tr>
<tr><td>120</td><td width="150"><span class="Monospace">KeyCode_F9</span></td>
<td>Constant for the <span class="Monospace">F9</span> key.</td></tr>
<tr><td>121</td><td width="150"><span class="Monospace">KeyCode_F10</span></td>
<td>Constant for the <span class="Monospace">F10</span> key.</td></tr>
<tr><td>122</td><td width="150"><span class="Monospace">KeyCode_F11</span></td>
<td>Constant for the <span class="Monospace">F11</span> key.</td></tr>
<tr><td>123</td><td width="150"><span class="Monospace">KeyCode_F12</span></td>
<td>Constant for the <span class="Monospace">F12</span> key.</td></tr>
<tr><td>124</td><td width="150"><span class="Monospace">KeyCode_F13</span></td>
<td>Constant for the <span class="Monospace">F13</span> key.</td></tr>
<tr><td>125</td><td width="150"><span class="Monospace">KeyCode_F14</span></td>
<td>Constant for the <span class="Monospace">F14</span> key.</td></tr>
<tr><td>126</td><td width="150"><span class="Monospace">KeyCode_F15</span></td>
<td>Constant for the <span class="Monospace">F15</span> key.</td></tr>
<tr><td>127</td><td width="150"><span class="Monospace">KeyCode_F16</span></td>
<td>Constant for the <span class="Monospace">F16</span> key.</td></tr>
<tr><td>128</td><td width="150"><span class="Monospace">KeyCode_F17</span></td>
<td>Constant for the <span class="Monospace">F17</span> key.</td></tr>
<tr><td>129</td><td width="150"><span class="Monospace">KeyCode_F18</span></td>
<td>Constant for the <span class="Monospace">F18</span> key.</td></tr>
<tr><td>130</td><td width="150"><span class="Monospace">KeyCode_F19</span></td>
<td>Constant for the <span class="Monospace">F19</span> key.</td></tr>
<tr><td>131</td><td width="150"><span class="Monospace">KeyCode_F20</span></td>
<td>Constant for the <span class="Monospace">F20</span> key.</td></tr>
<tr><td>132</td><td width="150"><span class="Monospace">KeyCode_F21</span></td>
<td>Constant for the <span class="Monospace">F21</span> key.</td></tr>
<tr><td>133</td><td width="150"><span class="Monospace">KeyCode_F22</span></td>
<td>Constant for the <span class="Monospace">F22</span> key.</td></tr>
<tr><td>134</td><td width="150"><span class="Monospace">KeyCode_F23</span></td>
<td>Constant for the <span class="Monospace">F23</span> key.</td></tr>
<tr><td>135</td><td width="150"><span class="Monospace">KeyCode_F24</span></td>
<td>Constant for the <span class="Monospace">F24</span> key.</td></tr>
<tr><td>144</td><td width="150"><span class="Monospace">KeyCode_NUMLOCK</span></td>
<td>Constant for the <span class="Monospace">NumLock</span> key.</td></tr>
<tr><td>145</td><td width="150"><span class="Monospace">KeyCode_SCROLL</span></td>
<td>Constant for the <span class="Monospace">Scroll</span> key.</td></tr>
<tr><td>173</td><td width="150"><span class="Monospace">KeyCode_VOLUME_MUTE</span></td>
<td>Constant for the <span class="Monospace">Volume Mute</span> key.</td></tr>
<tr><td>174</td><td width="150"><span class="Monospace">KeyCode_VOLUME_DOWN</span></td>
<td>Constant for the <span class="Monospace">Volume Down</span> key.</td></tr>
<tr><td>175</td><td width="150"><span class="Monospace">KeyCode_VOLUME_UP</span></td>
<td>Constant for the <span class="Monospace">Volume Up</span> key.</td></tr>
<tr><td>176</td><td width="150"><span class="Monospace">KeyCode_MEDIA_NEXT_TRACK</span></td>
<td>Constant for the <span class="Monospace">Media Next Track</span> key.</td></tr>
<tr><td>177</td><td width="150"><span class="Monospace">KeyCode_MEDIA_PREV_TRACK</span></td>
<td>Constant for the <span class="Monospace">Media Previous Track</span> key.</td></tr>
<tr><td>178</td><td width="150"><span class="Monospace">KeyCode_MEDIA_STOP</span></td>
<td>Constant for the <span class="Monospace">Media Stop</span> key.</td></tr>
<tr><td>179</td><td width="150"><span class="Monospace">KeyCode_MEDIA_PLAY_PAUSE</span></td>
<td>Constant for the <span class="Monospace">Media Pause</span> key.</td></tr>
</table>
</div></td></tr>
<tr><td width="150">AltPressed</td>
<td>Specifies whether the &lt;Alt&gt; key was pressed.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Boolean variable</a></td>
</tr>
</table>
</td></tr>
<tr><td width="150">CtrlPressed</td>
<td>Specifies whether the &lt;Ctrl&gt; key was pressed.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Boolean variable</a></td>
</tr>
</table>
</td></tr>
<tr><td width="150">ShiftPressed</td>
<td>Specifies whether the &lt;Shift&gt; key was pressed.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Boolean variable</a></td>
</tr>
</table>
</td></tr>
<tr><td width="150">Reserved</td>
<td>For future extensions. Always contains the value <a href="#" data-unresolved="1">Zero</a>.<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Variant variable</a></td>
</tr>
</table>
</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. If the value is <span class="Monospace">TRUE</span>, the shortcut is not returned to DIAdem. If the value is <span class="Monospace">FALSE</span>, the shortcut is passed on to DIAdem and the default action is executed. The shortcuts defined by the system, such as &lt;ALT&gt;-&lt;Esc&gt;, &lt;ALT&gt;-&lt;F4&gt;, &lt;ALT&gt;-&lt;Print&gt;, &lt;ALT&gt;-&lt;Space&gt;, &lt;Ctrl&gt;-&lt;Esc&gt;, &lt;Ctrl&gt;-&lt;F4&gt;, &lt;F1&gt;, &lt;Print&gt;, and &lt;Shift&gt;-&lt;Alt&gt;-&lt;Tab&gt;, cannot be disabled.</td></tr>
</table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
OnFilterKeyShortcut = "MyOnFilterKeyShortcut"

def MyOnFilterKeyShortcut(Panel, KeyCode, AltPressed, CtrlPressed, ShiftPressed, Reserved):
    MyOnFilterKeyShortcut = FALSE
    if ShiftPressed AND NOT AltPressed AND NOT CtrlPressed:
        # select KeyCode
        # case KeyCode_F1
        MyOnFilterKeyShortcut = TRUE
        # case else
```

---

*Source: `VarOff/OnFilterKeyShortcut.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

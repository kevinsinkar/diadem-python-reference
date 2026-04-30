---
title: "InputBoxDisp"
description: "Displays one or more prompts in a dialog and returns the contents of the input fields."
---

# InputBoxDisp

!!! abstract "Command &middot; `ComOff.chm`"
    Command: InputBoxDisp

Displays one or more prompts in a dialog and returns the contents of the input fields.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The function offers the possibility to have several input values entered with one call. If you pass a string array into the function via the <span class="Monospace">InputBoxDispTexts</span> parameter and the <span class="Monospace">InputBoxDispDefaultValues</span> parameter respectively, multiple input lines will be generated. If possible, both parameters should have the same size of the array, otherwise both will be reduced to the smallest size.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the function has provided multiple input fields, then the function creates an array of type <a href="#" data-unresolved="1">String variable</a> as a return parameter.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="200">InputBoxDispTexts</td>
<td>Determines the texts displayed in front of the dialog boxes. The maximum length depends on the width of the characters and is approximately 1024 characters.<br attr="ext"/><strong>a notice  </strong>If the function should only produce a single line of input, then you can enter the text directly as <a href="#" data-unresolved="1">String variable</a> specify. If there are several input fields, an array of type <a href="#" data-unresolved="1">String variable</a> is expected.<div id="exp_InputBoxDispTexts">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="200">[InputBoxDispTitle]</td>
<td>Specifies the dialog box title.<div id="exp_InputBoxDispTitle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="200">[InputBoxDispDefaultValues]</td>
<td>Determines the values that the InputBoxDisp method displays in the input boxes by default.<br attr="ext"/><strong>Note  </strong>If the function should only create a single input line, then you can specify the value directly as <a href="#" data-unresolved="1">String variable</a> . If there are several input fields, an array of type <a href="#" data-unresolved="1">String variable</a> is expected.<div id="exp_InputBoxDispDefaultValues">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant</a> type.</td></tr>
</table>
</div>

## Python example

```python
MyInput = dd.InputBoxDisp("Enter your name: ", "DIAdem", "Nobody")
if (not MyInput == None) :
    dd.Print("You entered: " + MyInput)
else:
    dd.Print("The dialog was canceled!")
```

```python
MyTexts = []
MyTexts.append("Value 1:")
MyTexts.append("Value 2:")
MyTexts.append("Value 3:")
MyDefaults = []
MyDefaults.append("100")
MyDefaults.append("200")
MyDefaults.append("300")
MyInputs = dd.InputBoxDisp(MyTexts, "DIAdem", MyDefaults)
if (not MyInputs == None) :
    for MyInputValue in MyInputs:
        dd.Print("Result: "+MyInputValue)
else:
    dd.Print("The dialog was canceled!")
```

---

*Source: `ComOff/InputBoxDisp.htm`*

---
title: "ToSudViewOb.GetArgument"
description: "Returns the transfer parameter of a user dialog box. When you call a user dialog box with SudDlgShow , you can transfer a parameter to the dialog box. However i"
---

# ToSudViewOb.GetArgument

!!! abstract "Method &middot; `Sudref.chm`"
    Method: GetArgument for Dialog

Returns the transfer parameter of a user dialog box. When you call a user dialog box with SudDlgShow , you can transfer a parameter to the dialog box. However if you use SudDlgCreate to generate a non-modal user dialog box, you cannot use the parameter transfer with the GetArgument method.

## Signature

```python
vGetArgument = Object.GetArgument()
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Class ArgumentHelper
# === Constructor and deconstructor ===
# === MyPara1 property ===
MyPara1  = MyPrivatPara1
End Property
MyPrivatPara1  = ParaNew1
End Property

# === MyPara2 property ===
MyPara2  = MyPrivatPara2
End Property
MyPrivatPara2  = ParaNew2
End Property
End Class

def Button1_EventClick(This):
    MyArguments = New ArgumentHelper
    MyArguments.MyPara1 = "Value 1"
    MyArguments.MyPara2 = "Value 2"
    if SudDlgShow("MySubDialog",ScriptReadPath + "Example.sud",MyArguments) == "IDOk":
        sgT = "Return values" + "\r\n" + MyArguments.MyPara1 + "\r\n" + MyArguments.MyPara2
        MsgBoxDisp(sgT)
```

```python
def Dialog_EventInitialize(This):
    oDlgParams = This.GetArgument()
    if not (oDlgParams is None) and not isNull(oDlgParams):
        sgT = "Input values" + "\r\n" + oDlgParams.MyPara1 + "\r\n" + oDlgParams.MyPara2
        MsgBoxDisp(sgT)

def OkButton_EventClick(This):
    # write back params
    oDlgParams.MyPara1 = "New Value 1"
    oDlgParams.MyPara2 = "New Value 1"
    Dialog.Ok
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"> <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/methods/SUD_method_GetArgument_ToSudViewOb.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

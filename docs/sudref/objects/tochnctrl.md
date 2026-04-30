---
title: "ToChnCtrl"
description: "The ChnCtrl object corresponds to the ChnCtrl control in a user dialog box. You use the ChnCtrl object to define a channel input field. As soon as you have ente"
---

# ToChnCtrl

!!! abstract "Object &middot; `Sudref.chm`"
    Object: ChnCtrl

The ChnCtrl object corresponds to the ChnCtrl control in a user dialog box. You use the ChnCtrl object to define a channel input field. As soon as you have entered at least two characters in the channel input field, an auto-complete window opens with a list of all channels in the Data Portal that contain these characters at any position in the group name or channel name without taking upper and lower case into account. If, for example, you have selected [Group index]/Channel name as syntax for the channel reference in the DIAdem settings and enter [1]/ , then DIAdem will display all channels of the first channel group. In addition, the channel input field in front of the text displays the type of the currently selected channel as a symbol. You can use the arrow keys or the mouse to select an entry from the auto-complete window. If you enter text that is not contained in a channel reference, DIAdem closes the auto-complete window.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
ChnCtrl1.Channel = dd.Data.GetChannel("[1]/Time")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tochnctrl-accelerator/">Accelerator</a> | <a href="../../properties/tochnctrl-backcolor/">BackColor</a> | <a href="../../properties/tochnctrl-bottom/">Bottom</a> | <a href="../../properties/tochnctrl-channel/">Channel</a> | <a href="../../properties/tochnctrl-cursorpointer/">CursorPointer</a> | <a href="../../properties/tochnctrl-enable/">Enable</a> | <a href="../../properties/tochnctrl-font/">Font</a> | <a href="../../properties/tochnctrl-forecolor/">ForeColor</a> | <a href="../../properties/tochnctrl-height/">Height</a> | <a href="../../properties/tochnctrl-left/">Left</a> | <a href="../../properties/tochnctrl-objectcode/">ObjectCode</a> | <a href="../../properties/tochnctrl-objecttype/">ObjectType</a> | <a href="../../properties/tochnctrl-readonly/">ReadOnly</a> | <a href="../../properties/tochnctrl-right/">Right</a> | <a href="../../properties/tochnctrl-tabstop/">TabStop</a> | <a href="../../properties/tochnctrl-tag/">Tag</a> | <a href="../../properties/tochnctrl-text/">Text</a> | <a href="../../properties/tochnctrl-top/">Top</a> | <a href="../../properties/tochnctrl-visible/">Visible</a> | <a href="../../properties/tochnctrl-width/">Width</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tochnctrl-layername/">LayerName</a> | <a href="../../methods/tochnctrl-move/">Move</a> | <a href="../../methods/tochnctrl-refresh/">Refresh</a> | <a href="../../methods/tochnctrl-runchange/">RunChange</a> | <a href="../../methods/tochnctrl-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tochnctrl-runinitialize/">RunInitialize</a> | <a href="../../methods/tochnctrl-setfocus/">SetFocus</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewob/">Dialog</a>.<a href="../../methods/tosudviewob-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToChnCtrl.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "ListItems"
description: "Collection of all selection terms of a selection list or a radio button in user dialog boxes."
---

# ListItems

!!! abstract "Collection &middot; `Sudref.chm`"
    Collection: ListItems

Collection of all selection terms of a selection list or a radio button in user dialog boxes.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>The methods <span class="Monospace">Add</span>, <span class="Monospace">Remove</span>, and <span class="Monospace">RemoveAll</span> are not available for the controls <a href="../../objects/tovarcombort/">EnumComboBox</a>, <a href="../../objects/tovarlistboxrt/">EnumListBox</a>, and <a href="../../objects/toradiort/">RadioButton</a>.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, ComboBox1.Items.Count + 1):
    MsgBoxDisp(i + ", " + ComboBox1.Items(i).Text)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tolistitems-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tolistitems-add/">Add</a> | <a href="../../methods/tolistitems-item/">Item</a> | <a href="../../methods/tolistitems-remove/">Remove</a> | <a href="../../methods/tolistitems-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/combobox/">ComboBox &lt;XTable&gt;</a>.<a href="../../methods/xtable-items-3/">Items</a> | <a href="../../objects/tocombort/">ComboBox</a>.<a href="../../methods/tocombort-items/">Items</a> | <a href="../../objects/tovarcombort/">EnumComboBox</a>.<a href="../../methods/tovarcombort-items/">Items</a> | <a href="../../objects/tovarlistboxrt/">EnumListBox</a>.<a href="../../methods/tovarlistboxrt-items/">Items</a> | <a href="../../objects/listbox/">ListBox &lt;XTable&gt;</a>.<a href="../../methods/xtable-items-4/">Items</a> | <a href="../../objects/tolistboxrt/">ListBox</a>.<a href="../../methods/tolistboxrt-items/">Items</a> | <a href="../../objects/toradiort/">RadioButton</a>.<a href="../../methods/toradiort-items/">Items</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToListItems.HTM`&nbsp;&middot;&nbsp;Python translated from VBS*

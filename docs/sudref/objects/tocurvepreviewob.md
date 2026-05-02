---
title: "ToCurvePreviewOb"
description: "The CurvePreview object corresponds to the CurvePreview control in a user dialog box. Use the Curve2DPreview object to define a curve preview to be displayed in"
---

# ToCurvePreviewOb

!!! abstract "Object &middot; `Sudref.chm`"
    Object: Curve2DPreview

!!! note "Context: SUD dialog editor"
    Examples in this section reference dialog-control identifiers like
    `Cell`, `Table1`, `ListBox1`, `ChnComboBox1`, etc. that exist as
    global-script-engine names **only when DIAdem has loaded a SUD
    dialog file containing those controls**. They are not accessible
    from standalone external Python; run these examples inside DIAdem's
    SUD editor, or use `dd.SudDlgCreate(...)` and `dd.SudDlgShow(...)`
    to create a dialog instance whose `.GetControl("<name>")` you can
    access.  See the [Runtime gotchas](../../getting-started.md#1-the-dispatch-surface-is-panel-conditional) section for the full panel-conditional dispatch story.

The CurvePreview object corresponds to the CurvePreview control in a user dialog box. Use the Curve2DPreview object to define a curve preview to be displayed in the dialog box. Use the Curves property to specify which channels or channel pairs to display in the curve preview.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Curve2DPreview1.Curves.RemoveAll
oMyCurve = Curve2DPreview1.Curves.Add("[1]/[1]","[1]/[2]")
oMyCurve.Color = 16711680
oMyCurve.Type = 1  # 1=Spikes
Curve2DPreview1.Refresh
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/tocurvepreviewob-axistextcolor/">AxisTextColor</a> | <a href="../../properties/tocurvepreviewob-backcolor/">BackColor</a> | <a href="../../properties/tocurvepreviewob-bottom/">Bottom</a> | <a href="../../properties/tocurvepreviewob-cursorpointer/">CursorPointer</a> | <a href="../../properties/tocurvepreviewob-curves/">Curves</a> | <a href="../../properties/tocurvepreviewob-height/">Height</a> | <a href="../../properties/tocurvepreviewob-labelvisible/">LabelVisible</a> | <a href="../../properties/tocurvepreviewob-left/">Left</a> | <a href="../../properties/tocurvepreviewob-legendvisible/">LegendVisible</a> | <a href="../../properties/tocurvepreviewob-objectcode/">ObjectCode</a> | <a href="../../properties/tocurvepreviewob-objecttype/">ObjectType</a> | <a href="../../properties/tocurvepreviewob-right/">Right</a> | <a href="../../properties/tocurvepreviewob-tag/">Tag</a> | <a href="../../properties/tocurvepreviewob-tooltiptext/">ToolTipText</a> | <a href="../../properties/tocurvepreviewob-top/">Top</a> | <a href="../../properties/tocurvepreviewob-visible/">Visible</a> | <a href="../../properties/tocurvepreviewob-width/">Width</a> | <a href="../../properties/tocurvepreviewob-xaxisscalingtype/">XAxisScalingType</a> | <a href="../../properties/tocurvepreviewob-yaxisscalingtype/">YAxisScalingType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/tocurvepreviewob-layername/">LayerName</a> | <a href="../../methods/tocurvepreviewob-move/">Move</a> | <a href="../../methods/tocurvepreviewob-refresh/">Refresh</a> | <a href="../../methods/tocurvepreviewob-runcustomaction/">RunCustomAction</a> | <a href="../../methods/tocurvepreviewob-runinitialize/">RunInitialize</a></p></div>
<div class="Events">
<h2>Events</h2>
<p><a href="../../events/eventcustomaction-eventcustomaction/">EventCustomAction</a> | <a href="../../events/eventinitialize-eventinitialize/">EventInitialize</a> | <a href="../../events/eventprepaint-eventprepaint/">EventPrePaint</a> | <a href="../../events/eventpostpaint-eventpostpaint/">EventPostPaint</a> | <a href="../../events/eventrefresh-eventrefresh/">EventRefresh</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/controls/">Controls</a>.<a href="../../methods/tocmdtarget-item/">Item</a> | <a href="../tosudviewobint/">Dialog &lt;NonModal&gt;</a>.<a href="../../methods/tosudviewobint-getcontrol/">GetControl</a> | <a href="../tosudviewob/">Dialog</a>.<a href="../../methods/tosudviewob-getcontrol/">GetControl</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="../../collections/curves/">Curves</a> | <a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Checking a User Dialog Box Entry</a> | <a href="#" data-unresolved="1">Creating a Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a Procedure in the Script of a User Dialog Box</a> | <a href="#" data-unresolved="1">Creating a User Dialog Box without Linking Variables</a> | <a href="#" data-unresolved="1">Creating an Extended Table</a> | <a href="#" data-unresolved="1">Displaying Graphics in Selection Lists</a> | <a href="#" data-unresolved="1">Enabling Controls</a> | <a href="#" data-unresolved="1">Responding to User Entries in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Saving and Restoring the Last Dialog Box Position</a> | <a href="#" data-unresolved="1">Saving Control Groups for User Dialog Boxes</a> | <a href="#" data-unresolved="1">Specifying the Default Button</a> | <a href="#" data-unresolved="1">Tabulator Order in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using a Script to Fill a Selection List</a> | <a href="#" data-unresolved="1">Using Channel Selection Lists</a> | <a href="#" data-unresolved="1">Using Hotkeys in a User Dialog Box</a> | <a href="#" data-unresolved="1">Using the Flex Properties</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking Dialog Box Entries</a> | <a href="#" data-unresolved="1">Dynamic User Dialog Box</a> | <a href="#" data-unresolved="1">Translating User Dialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box for Entering Text and Numbers</a> | <a href="#" data-unresolved="1">User Dialog Box for Sequence Control</a> | <a href="#" data-unresolved="1">User Dialog Box in DIAdem VIEW</a> | <a href="#" data-unresolved="1">User Dialog Box in VIEW for the Calculation of the FFT and Harmonic Frequencies</a> | <a href="#" data-unresolved="1">User Dialog Box with Changing Background Color</a> | <a href="#" data-unresolved="1">User Dialog Box with Curve Preview and Slider Control</a> | <a href="#" data-unresolved="1">User Dialog Box with Extended Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Scalable Table</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Selection Lists</a> | <a href="#" data-unresolved="1">User Dialog Box with Subdialog Boxes</a> | <a href="#" data-unresolved="1">User Dialog Box with Tables</a> | <a href="#" data-unresolved="1">User Dialog Box with Tree</a> | <a href="#" data-unresolved="1">Wizard for Tolerance Evaluation</a></p>
</div>
</div>

---

*Source: `Sudref/objects/SUD_Objects_ToCurvePreviewOb.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

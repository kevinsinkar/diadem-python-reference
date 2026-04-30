---
title: "ITDMTimeDisp"
description: "The USITimeDisp object provides date and time information."
---

# ITDMTimeDisp

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: UsiTimeDisp

The USITimeDisp object provides date and time information.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  You can also create a USITimeDisp object with the <a href="../../../comoff/commands/createtime/">CreateTime</a> command.</td></tr></table>
</div>

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyQueryForm.Search()
oMyResultsList = oMyCurrDataProvider.ResultsList
for Element in oMyResultsList.ResultsElements:
    if Element.IsKindOf(dd.eSearchFile) :
        oMyTime = Element.Properties("CreateTime").Value
        dd.MsgBoxDisp("name: " + Element.Name + "\r\n" + "Year: " + oMyTime.Year)
    else:
        dd.MsgBoxDisp("No File")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmtimedisp-day/">Day</a> | <a href="../../properties/itdmtimedisp-fraction/">Fraction</a> | <a href="../../properties/itdmtimedisp-hour/">Hour</a> | <a href="../../properties/itdmtimedisp-microsecond/">Microsecond</a> | <a href="../../properties/itdmtimedisp-millisecond/">Millisecond</a> | <a href="../../properties/itdmtimedisp-minute/">Minute</a> | <a href="../../properties/itdmtimedisp-month/">Month</a> | <a href="../../properties/itdmtimedisp-nanosecond/">Nanosecond</a> | <a href="../../properties/itdmtimedisp-second/">Second</a> | <a href="../../properties/itdmtimedisp-secondsfrom0000/">SecondsFrom0000</a> | <a href="../../properties/itdmtimedisp-secondsfrom1904/">SecondsFrom1904</a> | <a href="../../properties/itdmtimedisp-variantdate/">VariantDate</a> | <a href="../../properties/itdmtimedisp-year/">Year</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmtimedisp-getlocaltime/">GetLocalTime</a> | <a href="../../methods/itdmtimedisp-getutc/">GetUTC</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmdatafinderstatistics/">DataFinderStatistics</a>.<a href="../../properties/itdmdatafinderstatistics-lastcompleteindexing/">LastCompleteIndexing</a> | <a href="./">UsiTimeDisp</a>.<a href="../../methods/itdmtimedisp-getlocaltime/">GetLocalTime</a> | <a href="./">UsiTimeDisp</a>.<a href="../../methods/itdmtimedisp-getutc/">GetUTC</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Configuring the Search Results</a> | <a href="#" data-unresolved="1">Defining Search Areas</a> | <a href="#" data-unresolved="1">Executing a Search with OR Operations</a> | <a href="#" data-unresolved="1">Executing a Text Search</a> | <a href="#" data-unresolved="1">Indexing Search Areas</a> | <a href="#" data-unresolved="1">Optimizing Custom Properties</a> | <a href="#" data-unresolved="1">Saving and Loading a Search Query</a> | <a href="#" data-unresolved="1">Searching for Data on a Different Computer in the Network</a> | <a href="#" data-unresolved="1">Searching for Multiple Properties</a> | <a href="#" data-unresolved="1">Sorting Search Results before Executing a Search</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Brake Tests for Trucks</a> | <a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a> | <a href="#" data-unresolved="1">Combining DataFinder Search Results</a> | <a href="#" data-unresolved="1">Context Menu for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Creating ATFX Files from the Context Menu of an ASAM Data Store</a> | <a href="#" data-unresolved="1">Customized User Interface</a> | <a href="#" data-unresolved="1">Evaluation Wizard for the Search Results of the DataFinder</a> | <a href="#" data-unresolved="1">Filtering Data with a Dialog Box</a> | <a href="#" data-unresolved="1">Filtering Data without a Dialog Box</a> | <a href="#" data-unresolved="1">Search and Evaluation Functions in User Dialog Boxes</a> | <a href="#" data-unresolved="1">Searching for and Evaluating Channels</a> | <a href="#" data-unresolved="1">Searching for Channels in the NAVIGATOR</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed" in Data Stores</a> | <a href="#" data-unresolved="1">Searching for Data Sets Marked "Failed"</a> | <a href="#" data-unresolved="1">Searching for Properties and Evaluating the Associated Channels</a> | <a href="#" data-unresolved="1">Varying Browse Settings of a Data Store</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMTimeDisp.htm`*

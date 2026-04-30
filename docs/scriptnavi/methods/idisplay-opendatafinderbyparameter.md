---
title: "IDisplay.OpenDataFinderByParameter"
description: "Uses the specified parameters to open a connection to a DataFinder instance in the DIAdem NAVIGATOR interface."
---

# IDisplay.OpenDataFinderByParameter

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: OpenDataFinderByParameter for Display

Uses the specified parameters to open a connection to a DataFinder instance in the DIAdem NAVIGATOR interface.

## Signature

```python
bOpenDataFinderByParameter = Object.OpenDataFinderByParameter(ParamOrServerName, DataFinderName, ConnectionTimeout, QueryTimeout)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Instead of the <span class="Monospace">OpenDataFinderByParameter</span> method, you can use the associated urf file to open the connection to a DataFinder instance. Double-click the urf file to register it on the client computer. You can also use the <a href="../../objects/inavigator/">Navigator</a>.<a href="../../objects/inavigatorsettings/">Settings</a>.<a href="../inavigatorsettings-registerdataprovider/">RegisterDataProvider</a> method to register the DataFinder instance.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If DIAdem cannot execute the <span class="Monospace">OpenDataFinderByParameter</span> method successfully, DIAdem fills the VBS error object and terminates the script. DIAdem writes further information into a logfile and displays a dialog box that contains further information on the error.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Use <span class="Monospace">Navigator.Display.CurrDataFinder</span> to access the DataFinder object.</td></tr></table>
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <span class="Monospace">GetDataFinder</span> method to determine the associated DataFinder without interface for a DataFinder, which already has an open interface. Use the <span class="Monospace">ConnectDataFinder</span> method to work directly with a DataFinder without a user interface.</td></tr></table>
</div>

## Python example

```python
dd.Navigator.Display.OpenDataFinderByParameter("MyServer", "My DataFinder Instance", 10,20)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_OpenDataFinderByParameter_IDisplay.htm`*

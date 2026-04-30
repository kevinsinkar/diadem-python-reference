---
title: "INavigator.ConnectDataFinderByParameter"
description: "Opens a connection to a DataFinder on a different server."
---

# INavigator.ConnectDataFinderByParameter

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: ConnectDataFinderByParameter for Navigator

Opens a connection to a DataFinder on a different server.

## Signature

```python
return_value = obj.ConnectDataFinderByParameter(ParamOrServerName, DataFinderName, [ConnectTimeout], [QueryTimeout])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Instead of the <span class="Monospace">ConnectDataFinderByParameter</span> method, you can use the associated urf file to open the connection to a DataFinder instance. Double-click the urf file to register it on the client computer. You can also use the <a href="../../objects/inavigator/">Navigator</a>.<a href="../../objects/inavigatorsettings/">Settings</a>.<a href="../inavigatorsettings-registerdataprovider/">RegisterDataProvider</a> method to register the DataFinder instance.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinderByParameter("MyOwnDataFinder","MyDataFinder",5,5)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_ConnectDataFinderByParameter_INavigator.htm`*

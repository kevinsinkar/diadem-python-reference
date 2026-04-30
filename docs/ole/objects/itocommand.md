---
title: "ITOCommand"
description: "The TOCommand interface contains all the methods for controlling DIAdem commands, as well as the access to individual variables. Always use the bInterfaceLocked"
---

# ITOCommand

!!! abstract "Object &middot; `OLE.chm`"
    Object: TOCommand

The TOCommand interface contains all the methods for controlling DIAdem commands, as well as the access to individual variables. Always use the bInterfaceLocked property to request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an OLE command to DIAdem although the property has the value True , the behavior of DIAdem is unpredictable.

## Python example

```python
import win32com
oDIAdem = win32com.client.Dispatch("DIAdem.TOCommand")
if not oDIAdem.bInterfaceLocked :
    iSuccess = oDIAdem.CmdExecuteSync("wndshow('shell','normal')")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itocommand-bdontcloseapplication/">bDontCloseApplication</a> | <a href="../../properties/itocommand-binterfacelocked/">bInterfaceLocked</a> | <a href="../../properties/itocommand-bnoactivitydisplay/">bNoActivityDisplay</a> | <a href="../../properties/itocommand-bnodialogdisplay/">bNoDialogDisplay</a> | <a href="../../properties/itocommand-bnoerrordisplay/">bNoErrorDisplay</a> | <a href="../../properties/itocommand-bnoinfodisplay/">bNoInfoDisplay</a> | <a href="../../properties/itocommand-bnomsgdisplay/">bNoMsgDisplay</a> | <a href="../../properties/itocommand-bnowarningdisplay/">bNoWarningDisplay</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itocommand-boolvarget/">BoolVarGet</a> | <a href="../../methods/itocommand-boolvarset/">BoolVarSet</a> | <a href="../../methods/itocommand-cmdexecuteasync/">CmdExecuteAsync</a> | <a href="../../methods/itocommand-cmdexecutesync/">CmdExecuteSync</a> | <a href="../../methods/itocommand-doublevarget/">DoubleVarGet</a> | <a href="../../methods/itocommand-doublevarset/">DoubleVarSet</a> | <a href="../../methods/itocommand-integervarget/">IntegerVarGet</a> | <a href="../../methods/itocommand-integervarset/">IntegerVarSet</a> | <a href="../../methods/itocommand-novalueget/">NoValueGet</a> | <a href="../../methods/itocommand-novalueset/">NoValueSet</a> | <a href="../../methods/itocommand-textvarget/">TextVarGet</a> | <a href="../../methods/itocommand-textvarset/">TextVarSet</a> | <a href="../../methods/itocommand-variantvarget/">VariantVarGet</a> | <a href="../../methods/itocommand-variantvarset/">VariantVarSet</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `OLE/objects/OLE_Objects_ITOCommand.htm`*

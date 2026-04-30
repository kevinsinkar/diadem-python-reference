---
title: "Objects (OLE Automation)"
---

# Objects

2 objects from `OLE.chm`.

| Name | Summary |
| --- | --- |
| [`ITOCommand`](itocommand.md) | The TOCommand interface contains all the methods for controlling DIAdem commands, as well as the access to individual variables. Always use the bInterfaceLocked property to request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an OLE command to DIAdem although the property has the value True , the behavior of DIAdem is unpredictable. |
| [`ITODataSheet`](itodatasheet.md) | The interface TODataSheet facilitates access to the DIAdem data area. Always use the bInterfaceLocked property to request the status of the DIAdem OLE interfaces before you execute an OLE command. If you send an OLE command to DIAdem although the property has the value True , the behavior of DIAdem is unpredictable. |

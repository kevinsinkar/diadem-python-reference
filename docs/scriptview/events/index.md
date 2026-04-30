---
title: "Events (VIEW Object Model)"
---

# Events

9 events from `Scriptview.chm`.

| Name | Summary |
| --- | --- |
| [`ActiveSheetChanged.OnActiveSheetChanged`](activesheetchanged-onactivesheetchanged.md) | Runs in DIAdem VIEW when the active worksheet changes. |
| [`CursorChanged.OnCursorChanged`](cursorchanged-oncursorchanged.md) | Triggers when the cursor moves, the measurement mode or the cursor type changes, and when the active area changes, in DIAdem VIEW. |
| [`OnContextMenuPointSelected.OnContextMenuPointSelected`](oncontextmenupointselected-oncontextmenupointselected.md) | Is triggered when an item in a context menu is selected in DIAdem VIEW. |
| [`OnDblClick.OnDblClick`](ondblclick-ondblclick.md) | Is triggered when an area in double-clicked in DIAdem VIEW. |
| [`OnDrop.OnDrop`](ondrop-ondrop.md) | Is triggered in DIAdem VIEW when you drag and drop elements such as one or several channels, a channel group, or one or more properties from the Data Portal into an area. The area must be a Channel Table , 2D-Axis System , Bode , Polar , Orbit , Shaft Centerline , Contour , Graphics , Video , or a Textbox display type. The event is not triggered for the display types Map and Dialog Box . The event can only trigger if you can Drop data. The event is triggered if the cursor is above an area in DIAdem VIEW and you release the left mouse button. |
| [`OnDropAllowed.OnDropAllowed`](ondropallowed-ondropallowed.md) | Is triggered in DIAdem VIEW when you drag and drop elements such as one or several channels, a channel group, or one or more properties from the Data Portal into an area. The area must be empty or of the display type Channel Table , 2D Axis System , Bode , Polar , Orbit , Shaft Centerline , Bird's Eye View , Contour , Cascade , Graphic , Video or Textbox . The event is not triggered for the display types Map , Dialog Box and Python graphic . The event is triggered when you move the cursor over an area. Use this event to determine whether dropping onto an area is allowed. |
| [`OnLayoutLoaded.OnLayoutLoaded`](onlayoutloaded-onlayoutloaded.md) | Is triggered in DIAdem VIEW after a layout is loaded. |
| [`OnLegendClicked.OnLegendClicked`](onlegendclicked-onlegendclicked.md) | Is triggered in DIAdem if you left-click a legend. |
| [`OnShowingContextMenu.OnShowingContextMenu`](onshowingcontextmenu-onshowingcontextmenu.md) | Is triggered when a context menu displays in an area in DIAdem VIEW. |

---
title: Deprecated Control Pattern Functions
description: Deprecated Control Pattern Functions
ms.assetid: 06434b07-7592-4909-8c4e-064382bdbf98
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Deprecated Control Pattern Functions

> [!Note]  
> The control pattern functions described in this section are deprecated. Client applications should use the Component Object Model (COM) interfaces described in the following sections:
>
> -   [UI Automation Element Interfaces for Clients](uiauto-entry-uiautoclientinterfaces.md)
> -   [Property Condition Interface for Clients](uiauto-client-propconditioninterfaces.md)
> -   [Control Pattern Interfaces for Clients](uiauto-client-controlpatterninterfaces.md)
> -   [Event Handling Interfaces for Clients](uiauto-client-eventhandlinginterfaces.md)
> -   [Proxy Factory Interfaces for Clients](uiauto-client-proxyfactoryinterfaces.md)

 

## In this section



<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Function</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>[<strong>DockPattern_SetDockPosition</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-dockpattern_setdockposition)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the Microsoft UI Automation COM interfaces instead.
</blockquote>
<br/> Docks the UI Automation element at the requested <em>dockPosition</em> within a docking container.<br/></td>
</tr>
<tr class="even">
<td>[<strong>ExpandCollapsePattern_Collapse</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-expandcollapsepattern_collapse)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Hides all descendant nodes, controls, or content of the UI Automation element.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>ExpandCollapsePattern_Expand</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-expandcollapsepattern_expand)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Expands a control on the screen so that it shows more information.<br/></td>
</tr>
<tr class="even">
<td>[<strong>GridPattern_GetItem</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-gridpattern_getitem)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Gets the node for an item in a grid.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>InvokePattern_Invoke</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-invokepattern_invoke)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Sends a request to activate a control and initiate its single, unambiguous action.<br/></td>
</tr>
<tr class="even">
<td>[<strong>ItemContainerPattern_FindItemByProperty</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-itemcontainerpattern_finditembyproperty)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Retrieves a node within a containing node, based on a specified property value.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>LegacyIAccessiblePattern_DoDefaultAction</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-legacyiaccessiblepattern_dodefaultaction)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Performs the Microsoft Active Accessibility default action for the element.<br/></td>
</tr>
<tr class="even">
<td>[<strong>LegacyIAccessiblePattern_GetIAccessible</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-legacyiaccessiblepattern_getiaccessible)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Retrieves an [<strong>IAccessible</strong>](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) object that corresponds to the UI Automation element.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>LegacyIAccessiblePattern_Select</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-legacyiaccessiblepattern_select)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Performs a Microsoft Active Accessibility selection.<br/></td>
</tr>
<tr class="even">
<td>[<strong>LegacyIAccessiblePattern_SetValue</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-legacyiaccessiblepattern_setvalue)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Sets the Microsoft Active Accessibility value property for the node.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>MultipleViewPattern_GetViewName</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-multipleviewpattern_getviewname)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Retrieves the name of a control-specific view.<br/></td>
</tr>
<tr class="even">
<td>[<strong>MultipleViewPattern_SetCurrentView</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-multipleviewpattern_setcurrentview)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Sets a control to a different layout.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>RangeValuePattern_SetValue</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-rangevaluepattern_setvalue)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Sets the value of a control that has a numerical range.<br/></td>
</tr>
<tr class="even">
<td>[<strong>ScrollItemPattern_ScrollIntoView</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-scrollitempattern_scrollintoview)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Scrolls the content area of a container object in order to display the UI Automation element within the visible region (viewport) of the container.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>ScrollPattern_Scroll</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-scrollpattern_scroll)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Scrolls the currently visible region of the content area the specified [<strong>ScrollAmount</strong>](/windows/desktop/api/UIAutomationCore/ne-uiautomationcore-scrollamount), horizontally, vertically, or both.<br/></td>
</tr>
<tr class="even">
<td>[<strong>ScrollPattern_SetScrollPercent</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-scrollpattern_setscrollpercent)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Scrolls a container to a specific position horizontally, vertically, or both.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>SelectionItemPattern_AddToSelection</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-selectionitempattern_addtoselection)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Adds an unselected element to a selection in a control.<br/></td>
</tr>
<tr class="even">
<td>[<strong>SelectionItemPattern_RemoveFromSelection</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-selectionitempattern_removefromselection)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Removes an element from the selection in a selection container.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>SelectionItemPattern_Select</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-selectionitempattern_select)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Selects an element in a selection container.<br/></td>
</tr>
<tr class="even">
<td>[<strong>SynchronizedInputPattern_Cancel</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-synchronizedinputpattern_cancel)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Causes the UI Automation provider to stop listening for mouse or keyboard input.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>SynchronizedInputPattern_StartListening</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-synchronizedinputpattern_startlistening)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Causes the UI Automation provider to start listening for mouse or keyboard input.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextPattern_get_DocumentRange</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textpattern_get_documentrange)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Gets the text range for the entire document.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextPattern_get_SupportedTextSelection</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textpattern_get_supportedtextselection)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Ascertains whether the text container's contents can be selected and deselected.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextPattern_GetSelection</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textpattern_getselection)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Gets the current range of selected text from a text container supporting the text pattern.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextPattern_GetVisibleRanges</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textpattern_getvisibleranges)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Retrieves an array of disjoint text ranges from a text container where each text range begins with the first partially visible line through to the end of the last partially visible line. For example, a multi-column layout where the columns are partially scrolled out of the visible area of the viewport and the content flows from the bottom of one column to the top of the next.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextPattern_RangeFromChild</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textpattern_rangefromchild)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Gets the text range that a given node spans.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextPattern_RangeFromPoint</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textpattern_rangefrompoint)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Retrieves the degenerate (empty) text range nearest to the specified screen coordinates.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_AddToSelection</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_addtoselection)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Adds to the existing collection of highlighted text in a text container that supports multiple, disjoint selections by highlighting supplementary text corresponding to the calling text range <em>Start</em> and <em>End</em> endpoints.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_Clone</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_clone)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Copies a text range.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_Compare</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_compare)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Compares two text ranges.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_CompareEndpoints</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_compareendpoints)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Returns a value indicating whether two text ranges have identical endpoints.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_ExpandToEnclosingUnit</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_expandtoenclosingunit)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Expands the text range to a larger or smaller unit such as Character, Word, Line, or Page.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_FindAttribute</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_findattribute)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Searches in a specified direction for the first piece of text supporting a specified text attribute.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_FindText</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_findtext)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Returns the first text range in the specified direction that contains the text the client is searching for.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_GetAttributeValue</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_getattributevalue)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Gets the value of an text attribute for a text range.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_GetBoundingRectangles</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_getboundingrectangles)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Retrieves the minimum number of bounding rectangles that can enclose the range, one rectangle per line.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_GetChildren</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_getchildren)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Returns all UI Automation elements contained within the specified text range.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_GetEnclosingElement</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_getenclosingelement)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Returns the node for the next smallest provider that covers the range.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_GetText</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_gettext)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Returns the text in a text range, up to a specified number of characters.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_Move</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_move)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Moves the text range the specified number of units requested by the client.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_MoveEndpointByRange</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_moveendpointbyrange)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Moves an endpoint of one range to the endpoint of another range.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_MoveEndpointByUnit</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_moveendpointbyunit)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Moves an endpoint of the range the specified number of units.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_RemoveFromSelection</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_removefromselection)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Removes the selected text, corresponding to the calling text range <em>TextPatternRangeEndpoint_Start</em> and <em>TextPatternRangeEndpoint_End</em> endpoints, from an existing collection of selected text in a text container that supports multiple, disjoint selections.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TextRange_ScrollIntoView</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_scrollintoview)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Scrolls the text so the specified range is visible in the viewport.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TextRange_Select</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-textrange_select)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Selects a text range.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TogglePattern_Toggle</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-togglepattern_toggle)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Toggles a control to its next supported state.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TransformPattern_Move</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-transformpattern_move)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Moves an element to a specified location on the screen.<br/></td>
</tr>
<tr class="even">
<td>[<strong>TransformPattern_Resize</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-transformpattern_resize)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Resizes an element on the screen.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>TransformPattern_Rotate</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-transformpattern_rotate)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Rotates an element on the screen.<br/></td>
</tr>
<tr class="even">
<td>[<strong>ValuePattern_SetValue</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-valuepattern_setvalue)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Sets the text value of an element.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>VirtualizedItemPattern_Realize</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-virtualizeditempattern_realize)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Makes the virtual item fully accessible as a UI Automation element.<br/></td>
</tr>
<tr class="even">
<td>[<strong>WindowPattern_Close</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-windowpattern_close)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Closes an open window.<br/></td>
</tr>
<tr class="odd">
<td>[<strong>WindowPattern_SetWindowVisualState</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-windowpattern_setwindowvisualstate)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Sets the visual state of a window; for example, to maximize a window.<br/></td>
</tr>
<tr class="even">
<td>[<strong>WindowPattern_WaitForInputIdle</strong>](/windows/desktop/api/UIAutomationCoreApi/nf-uiautomationcoreapi-windowpattern_waitforinputidle)<br/></td>
<td><blockquote>
[!Note]<br />
This function is deprecated. Client applications should use the UI Automation COM interfaces instead.
</blockquote>
<br/> Causes the calling code to block for the specified time or until the associated process enters an idle state, whichever completes first.<br/></td>
</tr>
</tbody>
</table>



 

## Related topics

<dl> <dt>

[UI Automation Clients](uiauto-entry-uiautoclientsforwin32apps.md)
</dt> </dl>

 

 





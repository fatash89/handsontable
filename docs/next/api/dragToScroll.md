---
title: DragToScroll
permalink: /next/api/drag-to-scroll
canonicalUrl: /api/drag-to-scroll
editLink: false
---

# DragToScroll

[[toc]]

## Description

Plugin used to scroll Handsontable by selecting a cell and dragging outside of the visible viewport.


## Members

### boundaries
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L40
  

_dragToScroll.boundaries : DOMRect_
Size of an element and its position relative to the viewport,
e.g. {bottom: 449, height: 441, left: 8, right: 814, top: 8, width: 806, x: 8, y:8}.


## Methods

### check
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L127
  

_dragToScroll.check(x, y)_
Checks if the mouse position (X, Y) is outside of the viewport and fires a callback with calculated X an Y diffs
between passed boundaries.


| Param | Type | Description |
| --- | --- | --- |
| x | `number` | Mouse X coordinate to check. |
| y | `number` | Mouse Y coordinate to check. |



### destroy
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L263
  

_dragToScroll.destroy()_
Destroys the plugin instance.



### disablePlugin
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L96
  

_dragToScroll.disablePlugin()_
Disables the plugin functionality for this Handsontable instance.



### enablePlugin
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L70
  

_dragToScroll.enablePlugin()_
Enables the plugin functionality for this Handsontable instance.



### isEnabled
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L63
  

_dragToScroll.isEnabled() ⇒ boolean_
Checks if the plugin is enabled in the handsontable settings. This method is executed in [Hooks#beforeInit](./Hooks/#beforeInit)
hook and if it returns `true` than the [enablePlugin](#DragToScroll+enablePlugin) method is called.



### setBoundaries
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L107
  

_dragToScroll.setBoundaries(boundaries)_
Sets the value of the visible element.


| Param | Type | Description |
| --- | --- | --- |
| boundaries | `DOMRect` | An object with coordinates compatible with DOMRect. |



### setCallback
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L116
  

_dragToScroll.setCallback(callback)_
Changes callback function.


| Param | Type | Description |
| --- | --- | --- |
| callback | `function` | The callback function. |



### updatePlugin
::: source-code-link https://github.com/handsontable/handsontable/blob/develop/src/plugins/dragToScroll/dragToScroll.js#L86
  

_dragToScroll.updatePlugin()_
Updates the plugin state. This method is executed when [Core#updateSettings](./Core/#updateSettings) is invoked.


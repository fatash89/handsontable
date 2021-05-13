---
title: Row freezing
metaTitle: Row freezing - Guide - Handsontable Documentation
permalink: /next/row-freezing
canonicalUrl: /row-freezing
tags:
  - fixing rows
  - pinning rows
---

# Row freezing

[[toc]]

Specify two fixed rows with `fixedRowsTop: 2`. You'll need horizontal scrollbars, so just set a container `width` and `overflow: hidden` in CSS.

::: example #example1
```js
const container = document.querySelector('#example1');

const hot1 = new Handsontable(container, {
  data: Handsontable.helper.createSpreadsheetData(100, 50),
  colWidths: 100,
  width: '100%',
  height: 320,
  rowHeaders: true,
  colHeaders: true,
  fixedRowsTop: 2,
  licenseKey: 'non-commercial-and-evaluation'
});
```
:::
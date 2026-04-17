# Vue Gantt Chart Selection Demo

A Vue 3 demo repository for Syncfusion Gantt row selection with sample task data.

## Overview

This repository contains a Vue app demonstrating Syncfusion Vue Gantt row selection with multiple selection and record logging.

## Project structure

- `src/App.vue`
- `src/data.js`
- `src/main.js`

## Features

- Row selection with toggle support
- Selected row index and record logging
- Nested task data

## Prerequisites

- Node.js 14+
- npm
- Vue CLI if required

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```
2. Add a Syncfusion license in `src/main.js`:
   ```js
   registerLicense("Your license key")
   ```
3. Start the app:
   ```bash
   npm run serve
   ```

## Usage

The Gantt chart uses:

- `allowSelection: true`
- `selectionSettings: { type: 'Multiple', mode: 'Row', enableToggle: true }`

The button logs selection via:

```js
let ganttObj = this.$refs.gantt.ej2Instances;
console.log(ganttObj.selectionModule.getSelectedRowIndexes())
console.log(ganttObj.selectionModule.getSelectedRecords())
```

## Notes

- Change `mode` to `Cell` for cell selection.
- Sample data is in `src/data.js`.
- Styles load from the Syncfusion CDN in `App.vue`.

## Dependencies

- `vue`
- `@syncfusion/ej2-vue-gantt`
- `@syncfusion/ej2-vue-buttons`

## Link

- Syncfusion selection docs: https://helpej2.syncfusion.com/vue/documentation/gantt/selection/selection

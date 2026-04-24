# Vue Gantt Chart Selection Demo

A Vue 3 sample application demonstrating row selection behavior in the Syncfusion Vue Gantt Chart component using hierarchical task data.

## Project Overview

The sample focuses on configuring selection behavior in the Vue Gantt Chart using built‑in selection settings. It demonstrates how to enable row selection with toggle support, handle multiple selected rows, and retrieve selection details from the Gantt instance for further processing or logging.

## Features

- Row selection with toggle support
- Multiple row selection configuration
- Programmatic access to selected row indexes and records
- Hierarchical task data rendering in the Gantt chart

## Prerequisites

- Node.js (LTS or later)
- npm
- Vue 3 development environment

## Setup

1. Install dependencies:

   ```bash
   npm install
   ```
2. Start the app:

   ```bash
   npm run serve
   ```

## Usage

The Gantt chart is configured with selection enabled using the following options:

   - allowSelection: true
   - selectionSettings with:
      - type: 'Multiple'
      - mode: 'Row'
      - enableToggle: true

A button in the UI retrieves the Gantt instance through a template reference and logs the selected row indexes and selected task records to the browser console.

## Notes

- Selection mode can be changed to Cell to enable cell‑level selection.
- Sample task data is loaded from a local data source.
- Syncfusion theme styles are referenced to apply consistent Gantt styling.

## Link

- Syncfusion selection docs: https://helpej2.syncfusion.com/vue/documentation/gantt/selection/selection

# Event API introduction

## Event API in Beta

Events APIs in Javascript provides a way of interacting between add-ins and users upon several objects. Each time certain types of changes occur in Excel, an event notification fires. By using the Excel JavaScript API, you can register event handlers that allow your add-in to automatically run a designated function when a specific event occurs. The following events are currently supported.

| Event | Description | Supported objects |
|:---------------|:-------------|:-----------|
| `onAdded` | Event that occurs when an object is added. | **WorksheetCollection** |
| `onActivated` | Event that occurs when an object is activated. | **WorksheetCollection**, **Worksheet** |
| `onDeactivated` | Event that occurs when an object is deactivated. | **WorksheetCollection**, **Worksheet** |
| `onChanged` | Event that occurs when data within cells is changed. | **Worksheet**, **Table**, **TableCollection** |
| `onSelectionChanged` | Event that occurs when the active cell or selected range is changed. | **Worksheet**, **Table** |

## Upcoming event API

More event APIs are under progress. If you think about event APIs lack in certain type of events, please fill out in the survey section.

| Event | Description | Supported objects |
|:---------------|:-------------|:-----------|
| `onAdded` | Event that occurs when an object is added. | **ChartCollction** |
| `onDeleted` | Event that occurs when an object is deleted. | **WorksheetCollection**, **ChartCollection** |
| `onActivated` | Event that occurs when an object is activated. | **ChartCollection**, **Chart** |
| `onDeactivated` | Event that occurs when an object is deactivated. | **ChartCollection**, **Chart** |
| `onCalculated` | Event that occurs when calculation is done in worksheet. | **Worksheet** |

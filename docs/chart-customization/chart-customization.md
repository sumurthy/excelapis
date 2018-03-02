# Chart Customization


The Excel JavaScript Library provides APIs to enable your add-in to customize a chart in worksheet. To understand the concepts and the terminology of chart, please see the following articles about how users customize chart through the Excel UI:

- [Create charts](https://support.office.com/en-us/article/231c42d2-5e58-40e1-99f0-cbe618cfee1d)
- [Format charts](https://support.office.com/en-us/article/92693043-1772-46a9-90e3-88c8c76084d8)
- [Add trendlines](https://support.office.com/en-us/article/6b72b363-aa05-4c93-8c5b-22c480eb6e1f)

## Programmatic add/delete/customize series in chart

The `Chart.series` property, which is a [ChartSeriesCollection](https://github.com/OfficeDev/office-js-docs/blob/ExcelJs_OpenSpec/reference/excel/chartseriescollection.md) object, is the entry point for programmatic control of series CRUD in a chart. There are two properties and five  in the `ChartSeriesCollection` object:

- `count` &#8212; Returns the number of series in the collection.
- `items` &#8212; A collection of chart series objects. See [ChartSeries](https://github.com/OfficeDev/office-js-docs/blob/ExcelJs_OpenSpec/reference/excel/chartseries.md).


> [!NOTE]
> Data validation added programmatically behaves just like manually added data validation. In particular, note that data validation is triggered only if the user directly types a value into a cell or copies and pastes a cell from elsewhere in the workbook and takes the **Values** paste option. If the user copies a cell and does a plain paste into a range with data validation, validation is not triggered.

### Creating validation rules

To add data validation to a range, your code must set the `rule` proeprty of the `DataValidation` object in `Range.dataValidation`. This takes a [DataValidationRule](https://dev.office.com/reference/add-ins/excel/datavalidationrule) object which has seven optional properties. *No more than one of these properties may be present in any `DataValidationRule` object.* The property that you include determines the type of validation.

## Programmatic add/delete/customize trendline in chart

TBD

## Programmatic customize axis in chart

TBD

## Programmatic customize title and data label in chart


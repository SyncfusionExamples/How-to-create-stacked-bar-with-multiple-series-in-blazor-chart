# How to Create Stacked bar with Multiple Series in Blazor Chart

## Overview

This sample demonstrates how to create multiple stacked bar groups using Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts). The implementation renders four stacking bar series and separates them into two independent stack groups by using the `StackingGroup` property.

By default, stacked series are combined into a single stack. This sample shows how multiple stacking groups can be displayed side by side for the same category, making it easier to compare related datasets while preserving individual stack totals. The example uses a categorical X-axis and binds data from an in-memory collection to multiple chart series.

## Key Features

- Uses the `SfChart` component to render chart visualizations.
- Configures the primary axis through `ChartPrimaryXAxis`.
- Sets `ValueType="Syncfusion.Blazor.Charts.ValueType.Category"` to display category-based data.
- Defines multiple chart series using `ChartSeriesCollection`.
- Uses `Type="ChartSeriesType.StackingBar"` to render stacked bar charts.
- Binds category values using the `XName` property.
- Binds numerical values using the `YName` property.
- Assigns data through the `DataSource` property.
- Creates independent stacking groups through the `StackingGroup` property.
- Demonstrates two separate stack groups: `Group1` and `Group2`.
- Uses a strongly typed `ChartData` class containing:
  - `X`
  - `YValue`
  - `YValue1`
  - `YValue2`
  - `YValue3`
- Populates the chart using an in-memory `List<ChartData>` data source.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the following project file:

   `MultipleStackingSeries/MultipleStackingSeries.csproj`

3. Restore NuGet packages when prompted.
4. Build the project.
5. Run the application using **Ctrl+F5**.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
cd MultipleStackingSeries
dotnet restore
dotnet run
```

5. Open the local URL displayed in the terminal after the application starts.

## Project Structure

`Pages/Index.razor` —- Contains the `SfChart` implementation, stacked bar series configuration, `StackingGroup` settings, data model, and sample data source.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the official Syncfusion documentation for Chart getting started and stacked chart configuration: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.
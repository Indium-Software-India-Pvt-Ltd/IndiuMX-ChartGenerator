# IndiuMX-ChartGenerator

\# Mendix Connector - ChartSVGGeneration

The **ChartSVGGeneration** Mendix connector is designed to create SVG images of area charts using JFreeChart and Apache Batik libraries. The connector generates customized area charts based on the provided dataset and allows users to define custom colors, fill, and stroke for the chart.

## Parameters

- **context**: The Mendix context in which the action is executed.
- **document**: A Mendix object representing the SVG document where the chart will be stored.
- **chartData**: A list of Mendix objects containing the chart data with attributes "Newdate" (representing the x-axis data) and "Value" (representing the y-axis data).
- **fillColor**: A string representing the custom fill color for the area chart. If not provided, the default color "#000000" (black) will be used.
- **strokeWidth**: A decimal value representing the custom stroke width for the chart lines.
- **seriesName**: A string representing the name of the data series.
- **xAxisLabel**: A string representing the label for the x-axis.
- **yAxisLabel**: A string representing the label for the y-axis.

## Execution

The connector processes the provided dataset to create an area chart using JFreeChart. It allows customization of the chart by specifying the fill color and stroke width. The resulting SVG image of the chart is then stored in the provided Mendix object as an image document.

## Code Overview

The provided code demonstrates the implementation of the **ChartSVGGeneration** connector. It uses JFreeChart to create an area chart based on the dataset. The chart is then customized with custom colors, fill, and stroke width using Apache Batik. The final SVG image is stored in the specified Mendix object as an image document.

Please note that the code is meant for illustration purposes only and should be further adapted and tested as per the specific requirements of your Mendix application.

## Getting Started

To use the **ChartSVGGeneration** connector, follow these steps:

1. Add the connector to your Mendix project.
2. Call the connector with the appropriate parameters.
3. Provide the dataset containing the chart data as Mendix objects.
4. Optionally, specify custom colors, fill, and stroke width for the chart.

## Examples

Example usage of the connector:

```java
ChartSVGGeneration connector = new ChartSVGGeneration(
    context,
    document,
    chartData,
    "#FF5733",
    BigDecimal.valueOf(2.5),
    "My Data Series",
    "X-Axis Label",
    "Y-Axis Label"
);

IMendixObject result = connector.executeAction();

Contributing
Contributions to the project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

License
This project is licensed under the MIT License.

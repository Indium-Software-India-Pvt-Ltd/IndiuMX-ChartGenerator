# IndiuMX-ChartGenerator

Mendix Connector - ChartSVGGeneration
The ChartSVGGeneration Mendix connector is designed to create SVG images of area charts using JFreeChart and Apache Batik libraries. The connector generates customized area charts based on the provided dataset and allows users to define custom colors, fill, and stroke for the chart.

Parameters
context: The Mendix context in which the action is executed.
document: A Mendix object representing the SVG document where the chart will be stored.
chartData: A list of Mendix objects containing the chart data with attributes "Newdate" (representing the x-axis data) and "Value" (representing the y-axis data).
fillColor: A string representing the custom fill color for the area chart. If not provided, the default color "#000000" (black) will be used.
strokeWidth: A decimal value representing the custom stroke width for the chart lines.
seriesName: A string representing the name of the data series.
xAxisLabel: A string representing the label for the x-axis.
yAxisLabel: A string representing the label for the y-axis.
Execution
The connector processes the provided dataset to create an area chart using JFreeChart. It allows customization of the chart by specifying the fill color and stroke width. The resulting SVG image of the chart is then stored in the provided Mendix object as an image document.

Code Overview
The provided code demonstrates the implementation of the ChartSVGGeneration connector. It uses JFreeChart to create an area chart based on the dataset. The chart is then customized with custom colors, fill, and stroke width using Apache Batik. The final SVG image is stored in the specified Mendix object as an image document.

Please note that the code is meant for illustration purposes only and should be further adapted and tested as per the specific requirements of your Mendix application.

For more information on using the connector and its parameters, please refer to the Mendix documentation.

The above README file provides a brief description of the ChartSVGGeneration Mendix connector and its parameters. It explains the purpose of the connector, the customization options available, and the steps involved in the execution of the connector. Additionally, it emphasizes the need for further adaptation and testing based on specific application requirements. The provided code is included in the README to serve as a reference for developers implementing the connector.

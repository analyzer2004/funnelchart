# Funnel Chart


**FunnelChart** shows values across multiple stages in a process. It helps you visualize a linear process that has sequential connected stages. Each funnel stage represents as different portions of the intake stage. The chart makes it easy to analyze where most dropouts are happening.

For live demos and sample codes, please see [Funnel Chart](https://observablehq.com/@analyzer2004/funnel-chart)

<img src="https://github.com/analyzer2004/funnelchart/blob/master/images/cover.png" width="768">

## API Reference
* **FunnelChart(container)** - Constructs a new instance of FunnelChart with default settings. The container can be an svg or g element.
* **size(_)** - Sets the dimensions of the chart to specified width, height and returns this chart.
* **options(options)** - Overrides the default settings and returns this chart.
  * options.**palette** - sets the color palette to the specified categorical color scheme.  
  * options.**style** - specifies the rendering style to *"2d"*, *"3d"* or *"flat"*. Default is 2d.
  * options.**streamlined** - a boolean value that specifies the data is streamlined or part-to-a-whole. Default is true (streamlined).
  * options.**percentage** - specifies the denominator of the percentage to the number of *"first"* or *"previous"* stage. Default is first.
  * options.**showPercentage** - sets whether the percentage is displayed.
* **font(font)** - Overrides the font settings and returns this chart.
  * font.**fontFamily** - sets the font. Default is sans-serif.
  * font.**size** -
    * size.**label** - sets the font size of labels. Default is 16.
    * size.**value** - sets the font size of values. Default is 16.
    * size.**percentage** - sets the font size of percentages. Default is 12.
* **field(field)** - Sets the field names for reading chart data and returns this chart.
  * field.**stage** - the field name of stage.
  * field.**value** - the field name of value.
* **tooltip(tooltip)** - Overrides the tooltip settings and returns this chart.
  * tooltip.**color** - sets the text color of tooltip.
  * tooltip.**boxColor** - sets the background color of the tooltip box.
  * tooltip.**boxOpacity** - sets the opacity of the tooltip box. Default is 0.8.
* **data(_)** - Sets the data and returns this chart.
* **render()** - Renders the chart and returns it's instance.
* **onhover(d)** - Occurs when user hover over a stage.
* **onclick(d)** - Occurs when user click on a stage.`
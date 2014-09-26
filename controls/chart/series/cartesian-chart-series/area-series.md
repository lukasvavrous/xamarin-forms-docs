---
title: AreaSeries
---
# LineSeries #

**RadCartesianChart** visualizes **AreaSeries** as an area on the chart that is enclosed by the coordinate axes and straight line segments that connect the data points represented by these series. The **AreaSeries** extend **CategoricalStrokedSeries**, so they are also **CategoricalSeries** and require one **CategoricalAxis** and one **NumricalAxis**.

## Example ##
Here is an example of how to create a basic RadCartesianChart with AreaSeries in xaml:

	<telerikChart:RadCartesianChart HeightRequest="600">
	  <telerikChart:RadCartesianChart.BindingContext>
	    <local:MainViewModel/>
	  </telerikChart:RadCartesianChart.BindingContext>
	  <telerikChart:RadCartesianChart.HorizontalAxis>
	    <telerikChart:CategoricalAxis/>
	  </telerikChart:RadCartesianChart.HorizontalAxis>
	  <telerikChart:RadCartesianChart.VerticalAxis>
	    <telerikChart:NumericalAxis/>
	  </telerikChart:RadCartesianChart.VerticalAxis>
	  <telerikChart:RadCartesianChart.Series>
	    <telerikChart:AreaSeries ItemsSource="{Binding CategoricalData}">
	      <telerikChart:AreaSeries.ValueBinding>
	        <telerikChart:PropertyNameDataPointBinding PropertyName="Value"/>
	      </telerikChart:AreaSeries.ValueBinding>
	      <telerikChart:AreaSeries.CategoryBinding>
	        <telerikChart:PropertyNameDataPointBinding PropertyName="Category"/>
	      </telerikChart:AreaSeries.CategoryBinding>
	    </telerikChart:AreaSeries>
	  </telerikChart:RadCartesianChart.Series>
	</telerikChart:RadCartesianChart>
Here is an example of how to create a RadCartesianChart with AreaSeries in code:

	var chart = new RadCartesianChart
	{
	    HorizontalAxis = new Telerik.XamarinForms.Chart.CategoricalAxis(),
	    VerticalAxis = new Telerik.XamarinForms.Chart.NumericalAxis(),
	    HeightRequest = 600,
	    BindingContext = new ViewModel()
	};

	var series = new Telerik.XamarinForms.Chart.AreaSeries();
	series.SetBinding(AreaSeries.ItemsSourceProperty, new Binding("CategoricalData"));	
	series.ValueBinding = new PropertyNameDataPointBinding("Value");
	series.CategoryBinding = new PropertyNameDataPointBinding("Category");
	
	chart.Series.Add(series);

![Basic AreaSeries]()
## Customization ##
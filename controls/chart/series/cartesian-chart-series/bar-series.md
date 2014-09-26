---
title: BarSeries
---
# BarSeries #

**RadCartesianChart** visualizes each data point from the **BarSeries** as a rectangle. These rectangles (or bars) can be displayed either horizontally, or vertically, depending on whether the **CategoricalAxis** is the vertical axis or the horizontal. When the horizontal axis is categorical, the rectangles are displayed vertically. This means that they have equal width while their height represents the numerical value of each of the data points. On the other hand, when the vertical axis is categorical, the rectangles have equal height, while their width represents the value of the data point. The **BarSeries** inherit from **CategoricalSeries** and require one **CategoricalAxis** and one **NumericalAxis**.
## Example ##
Here is an example of how to create a basic RadCartesianChart with BarSeries in xaml:

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
	    <telerikChart:BarSeries ItemsSource="{Binding CategoricalData}">
	      <telerikChart:BarSeries.ValueBinding>
	        <telerikChart:PropertyNameDataPointBinding PropertyName="Value"/>
	      </telerikChart:BarSeries.ValueBinding>
	      <telerikChart:BarSeries.CategoryBinding>
	        <telerikChart:PropertyNameDataPointBinding PropertyName="Category"/>
	      </telerikChart:BarSeries.CategoryBinding>
	    </telerikChart:BarSeries>
	  </telerikChart:RadCartesianChart.Series>
	</telerikChart:RadCartesianChart>
Here is an example of how to create a RadCartesianChart with BarSeries in code:

	var chart = new RadCartesianChart
	{
	    HorizontalAxis = new Telerik.XamarinForms.Chart.CategoricalAxis(),
	    VerticalAxis = new Telerik.XamarinForms.Chart.NumericalAxis(),
	    HeightRequest = 600,
	    BindingContext = new ViewModel()
	};

	var series = new Telerik.XamarinForms.Chart.BarSeries();
	series.SetBinding(BarSeries.ItemsSourceProperty, new Binding("CategoricalData"));	
	series.ValueBinding = new PropertyNameDataPointBinding("Value");
	series.CategoryBinding = new PropertyNameDataPointBinding("Category");
	
	chart.Series.Add(series);
Here is the sample data:
	

![Basic BarSeries]()
## Customization ##
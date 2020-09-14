---
title: Delete Appointment View
page_title: Xamarin Calendar Documentation | Scheduling UI
description: Check our &quot;Scheduling UI Delete Appointment View&quot; documentation article for Telerik Calendar for Xamarin control.
position: 3
slug: calendar-delete-appointment-view
---

# Delete Appointment View

DeleteAppointmentView – view for choosing appointment deleting options.

## Visual Structure of Delete Appointment View

![Scheduling UI Delete Appointment View](images/calendar-delete-appointment-view.png)

## Control Template

> The control template for the **DeleteAppointmentView** can be found at the [following location in our SDKBrowser Application](https://github.com/telerik/xamarin-forms-sdk/blob/master/XamarinSDK/SDKBrowser/SDKBrowser/Examples/CalendarControl/SchedulingCategory/SchedulingUIViews/DeleteAppointmentView.xaml).

## Customization Properties 

* **ControlTemplate**(*ControlTemplate*): Defines the control template of the DeleteAppointmentView.
* **BackgroundColor**(*Xamarin.Forms.Color*): Defines the background color of the DeleteAppointmentView.

>important These properties or the ControlTemplates can be changed by applying style with TargetType="telerikInput:DeleteAppointmentView" in the resources of the “App.xaml” file of your application. 

### Example:

```XAML
<Style TargetType="telerikInput:DeleteAppointmentView">
    <Setter Property="BackgroundColor" Value="Red"/>
</Style>
```

In addition you will need to add the following namespace: 

<snippet id='xmlns-telerikinput'/>

## See Also

* [Add Appointment View]({%slug calendar-add-appointment-view%})
* [Appointment Summery View]({%slug calendar-appointment-summary-view%})
* [Color Picker View]({%slug calendar-color-picker-view%})
* [Custom Recurrence View]({%slug calendar-custom-recurrence-view%})
* [Repeat Appointment View]({%slug calendar-repeat-appointment-view%})
* [End Repeat Appointment View]({%slug calendar-end-repeat-appointment-view%})
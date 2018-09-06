---
title: Overview
page_title: Overview
description: Introduces the RadAutoCompleteView for XamarinForms component
position: 0
slug: autocompleteview-overview
---

# Overview #

**RadAutoCompleteView for Xamarin** can automatically complete user input string by comparing the text being entered to all strings in the associated data source. The control has a number of advanced features such as different filtering options, tokens support and remote search, as well as full customization capabilities.

#### Figure 1: RadAutoCompleteView Overview

![AutoCompleteView Overview](images/autocompleteview-overview.png "AutoComplete Overview")

## Key features

* **Tokens Support**: With RadAutoCompleteView you could enable users to search for and select several items in one control. These items appear as tokens that can easily be deselected using their close button. For more details on this check [here]({% slug autocomplete-key-features%}#tokens-support).
* **Filtering Options**:  You could define the filtering behavior to display all the matches that either “StartsWith” or “Contains” the typed symbols. Read [here]({% slug autocomplete-key-features%}#filtering-options) for more details on this.
* **Watermark**: Used to give guidance to the end user on what should be entered in the text input. Check [here]({% slug autocomplete-key-features%}#watermark) for more info.
* **NoResults Message**: NoResults message appears in the popup used for the list of suggestions whenever the control cannot find any matching items. Read more about this [here]({% slug autocomplete-key-features%}#noresults-message).
* **Customizable Items**: Whenever the default template does not fit a particular scenario you could use the SuggestionItemTemplate property to define a custom template. Read [here]({%slug autocomplete-suggestion-item-template %}) for detailed instructions on how you could apply it.
* **Remote Search**: Allows you to easily take the user input, trigger custom searching algorithm and assign the results to the ItemSource of the AutoComplete.
* **Show/Hide Suggestions**: AutoCompleteView provides the ability to show/hide all suggestions immediately when you focused on the input field.

## See Also

- [Getting Started]({% slug autocompleteview-getting-started %})
- [Key Features]({% slug autocompleteview-key-features %})
- [Tokens Support]({% slug autocompleteview-tokens-support %})
---
title: "Faceting - Filtering - Splitting"
teaching: 10
exercises: 5
questions:
- "What is a facet in OpenRefine?"
- "What is a filter in OpenRefine?"
- "How can I use filters and facets to explore data OpenRefine?"
- "How can I easily correct common data issues in my data with OpenRefine?"
objectives:
- "Explain what Facets and Filters are"
- "Answer simple questions about the content of a data set using Facets"
- "Use facets and filters to work with a subset of data"
- "Correct simple data problems through a facet"
- "Employ drop-downs to split values from one column into multiple columns."
keypoints:
- "You can use facets and filters to explore your data"
- "You can use facets and filters work with a subset of data in OpenRefine"
- "You can easily correct common data issues from a Facet"
---

## Facets
Facets are one of the most useful features of OpenRefine and can help both get an overview of the data in a project as well as helping you bring more consistency to the data.

A 'Facet' groups all the values that appear in a column, and then allow you to filter the data by these values and edit values across many records at the same time.

The simplest type of Facet is called a 'Text facet'. This simply groups all the text values in a column and lists each value with the number of records it appears in. The facet information always appears in the left hand panel in the OpenRefine interface.

To create a Text Facet for a column, click on the drop down menu at the top of the publisher column and choose `Facet -> Text Facet`. The facet will then appear in the left hand panel.

The facet consists of a list of values used in the data. You can filter the data displayed by clicking on one of these headings.

You can include multiple values from the facet in a filter at one time by using the `Include` option which appears when you put your mouse over a value in the Facet.

You can also `invert` the filter to show all records which do not match your selected values. This option appears at the top of the Facet panel when you select a value from the facet to apply as a filter.

>## Let's create a text facet
>1. Click on the drop down menu at the top of the publisher column and choose `Facet > Text Facet`. The facet will then appear in the left hand panel
>2. Filter by facet by clicking or `include`
>3. Select multiple values to `include`
>3. You can 'invert' your selections to `exclude`
>4. Include a value and then look at top to invert inclusion.
{: .checklist}

>## Which licences are used for articles in this file?
> Use a `text facet` for the `license` column and answer these questions:
>
>1. What is the most common Licence in the file?
>2. How many articles in the file don't have a licence assigned?
>
>>## Solution
>>* Create a facet for the 'Licence' column
>>* What is the most common Licence in the file? Answer: `CC BY`
>>* How many articles in the file don't have a licence assigned? Answer: **6**
>{: .solution}
{: .challenge}

## Working with filtered data
It is very important to note that when you have filtered the data displayed in OpenRefine, any operations you carry out will apply only to the rows that match the filter - that is the data currently being displayed.

## More on Facets
As well as 'Text facets' Refine also supports a range of other types of facet. These include:

* Numeric facets
* Timeline facets (for dates)
* Custom facets
* Scatterplot facets

Facets are intended to group together common values and OpenRefine limits the number of values allowed in a single facet to ensure the software does not perform slowly or run out of memory. If you create a facet where there are many unique values (for example, a facet on a 'book title' column in a data set that has one row per book) the facet created will be very large and may either slow down the application, or OpenRefine will not create the facet.

>## Find all publications without a DOI
>* Use the `Facet by blank` function to find all publications in this data set without a DOI
>
>>## Solution
>>
>>1. On the `DOI` column drop down and select `Customized facets > Facets by blank`
>>2. `True` means that it is blank, so you can:
>>    * Select `include` for true to winnow down the publications
>{: .solution}
{: .challenge}

## Amending data through facets
If you create a text facet you can edit the values in the facet to change the value for several records at the same time. To do this, simply mouse-over the value you want to edit and click the 'edit' option that appears.

This approach is useful in relatively small facets where you might have small variations through punctuation or typing errors etc. For example, a column that should contain only terms from a small restricted list such as days of the week or months of the year.

The list of values in the facet will update as you make edits.

>## Correct the Language values via a facet
>
>* `Text facet` on the `language` column and correct the variation in the `EN` and `English` values.
>
>>## Solution
>>1. Create a Text facet on the Language column
>>2. Notice that there is both `EN` and `English`
>>3. Put the mouse over the `English` value
>>4. Click `Edit`
>>5. Type `EN` and click `Apply`
>>6. See how the Language facet updates
>{: .solution}
{: .challenge}

## Split


If data in a column needs to be split into multiple columns, and the parts are separated by a common separator (say a comma, or a space), you can use that separator to divide up the pieces into their own columns.


1. Let us suppose we want to split the `Publisher` column into separate columns for Publisher and for Publishing Place. 
2. Click the down arrow at the top of the `Publisher` column. Choose `Edit Column` > `Split into several columns...`
3. In the pop-up, in the `Separator` box, replace the comma with a semi-colon (;).
4. Uncheck the box that says `Remove this column`.
5. Click `OK`. You'll get two new columns called `Publisher 1` and `Publisher 2`.


>## Exercise
>
>1. Change the name of the second new column to "PubPlace". 
>2. Change the name of the first new column to "Publisher". Is there a problem?
>
>>## Solution
>> 1. On the `Publisher 2` column, click the down arrow and then `Edit column` > `Rename this column`. Type "PubPlace" into the box
>> that appears. 
>> 2. Remove the original column `Edit column` > `Remove this column`. Then in the `Publisher 1` column, click the down arrow 
>> and then `Edit column` > `Rename this column`. Type "Publisher" into the box
>> that appears.
>{: .solution}
{: .challenge}

---
title: "Importing data into OpenRefine"
teaching: 5
exercises: 5
questions:
- "How do I get data into OpenRefine?"
- "How is data organised in OpenRefine?"
- "How do I access options to amend data in OpenRefine?"
- "What is the difference between Rows and Records in OpenRefine?"
- "How do I work with single cells that contain multiple values in a list?"
objectives:
- "Successfully import data into OpenRefine"
- Locate controls for navigating data in OpenRefine
- Find options to work with data through the OpenRefine dropdown menus
keypoints:
- "Use the `Create Project` option to import data"
- "You can control how data imports using options on the import screen"
- "OpenRefine uses rows and columns to display data"
- "Most options to work with data in OpenRefine are accessed through a drop down menu at the top of a data column"
- "When you select an option in a particular column (e.g. to make a change to the data), it will effect all the cells in that column"
---

## Importing data

>## What kinds of data files can I import?
>There are several options for getting your data set into OpenRefine. You can upload or import files in a variety of formats including:
>
>* TSV (tab-separated values)
>* CSV (comma-separated values)
>* Excel
>* JSON (javascript object notation)
>* XML
>* Google Spreadsheet
{: .callout}

>## Create your first OpenRefine project (using provided data)
>
> To import the data for the exercises below, run OpenRefine. *NOTE: If OpenRefine does not open in a browser window, open your browser and type the address <http://127.0.0.1:3333/> to take you to the OpenRefine interface.*
>
>1. Once OpenRefine is launched in your browser, click `Create Project` from the left hand menu and select `Get data from This Computer`
>2. Click `Choose Files` (or 'Browse', depending on your setup) and locate the file which you have downloaded called `doaj-article-sample.csv` *(if you haven't downloaded it yet, please see 'Downloading the data' in the Setup page [https://librarycarpentry.github.io/lc-open-refine/setup.html](https://librarycarpentry.github.io/lc-open-refine/setup.html))*
>3. Click `Next >>` - the next screen (see below) gives you options to ensure the data is imported into OpenRefine correctly. The options vary depending on the type of data you are importing.
>4. Click in the `Character encoding` box and set it to `UTF-8`
>5. Ensure the first row is used to create the column headings by checking the box `Parse next 1 line(s) as column headers`
>6. Make sure the `Parse cell text into numbers, dates, ...` box is not checked, so OpenRefine doesn't try to automatically detect numbers
>7. Once you are happy click the `Create Project >>` button at the top right of the screen. This will create the project and open it for you. Projects are saved as you work on them, there is no need to save copies as you go along.
>   
> ![Create project screen capture](../assets/img/openrefine_ui.png)
>
{: .checklist}

To open an existing project in OpenRefine you can click `Open Project` from the main OpenRefine screen (in the left hand menu). When you click this, you will see a list of the existing projects and can click on a project's name to open it.

### Going Further
* Look at the other options on the Import screen - try changing some of these options and see how that changes the Preview and how the data appears after import.
* Do you have access to JSON or XML data? If so the first stage of the import process will prompt you to select a 'record path' - that is the parts of the file that will form the data rows in the OpenRefine project.

## The layout of OpenRefine
OpenRefine displays data in a tabular format. Each row will usually represent a 'record' in the data, while each column represents a type of information. This is very similar to how you might view data in a spreadsheet or database. As with a spreadsheet, the individual bits of data live in 'cells' at the intersection of a row and a column.

OpenRefine only displays a limited number of rows of data at one time. You can adjust the number choosing between 5, 10 (the default), 25 and 50 at the top left of the table of data. You can navigate through the records by using the previous/next/first/last navigation options at the top right of the table of data.

## Working with data in OpenRefine
Most options to work with data in OpenRefine are accessed from drop down menus at the top of the data columns. When you select an option in a particular column (e.g. to make a change to the data), it will affect all the cells in that column. If you want to make changes across several columns, you will need to do this one column at a time.

